# Geolocate HAR file IPs

Welcome! This project is my solution for extracting IP addresses from a HAR file, finding out where they are in the world using the ipinfo.io API, and visualizing them on an interactive map made with Folium and Leaflet.

## How I Used This Project

1. **Install the required libraries:**
   - I made sure I had Python 3. I installed the needed packages with `pip install -r requirements.txt` (see the `requirements.txt` file for details).
2. **Get your HAR file ready:**
   - I downloaded a HAR file from my browser and updated the `HAR_FILE` variable in `scrape_har_locations.py` to point to my file.
3. **Run the script:**
   - I opened a terminal and ran: `python scrape_har_locations.py`
   - This created:
     - An interactive map: `outputs/ip_map.html`
     - A GeoJSON file: `outputs/ip_locations.geojson`

## What I'm Submitting

- **Screenshot:** See `webmap-screenshot.png` for a preview of the map I created.
- **GeoJSON:** The script generates `outputs/ip_locations.geojson` with all the geolocated IPs.
- **Web Map Files:**
  - The main file is `custom_map.html` (or `index.html` if you rename it).
  - **Note:** The HTML file is self-contained—everything (CSS and JavaScript) is right inside. To view the map, just download the folder, open the HTML file in your browser, and make sure the `outputs/ip_locations.geojson` file is in the right spot. No extra CSS or JS files needed!

## What's in This Folder?

- `scrape_har_locations.py` — The Python script that does all the work
- `custom_map.html` — The interactive web map (just open in your browser)
- `outputs/ip_locations.geojson` — The GeoJSON data for the map
- `webmap-screenshot.png` — A screenshot of the map
- `inputs/` — Where I put my HAR file

---
If you have any questions or run into any issues, feel free to reach out.