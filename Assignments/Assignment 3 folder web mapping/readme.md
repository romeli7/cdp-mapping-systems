# Geolocate HAR file IPs

Welcome! This project helps you extract IP addresses from a HAR file, find out where they are in the world using the ipinfo.io API, and see them on an interactive map made with Folium and Leaflet.

## How to Use This Project

1. **Install the required libraries:**
   - Make sure you have Python 3. You can install the needed packages with `pip install -r requirements.txt` (see the `requirements.txt` file for details).
2. **Get your HAR file ready:**
   - Download a HAR file from your browser and update the `HAR_FILE` variable in `scrape_har_locations.py` to point to your file.
3. **Run the script:**
   - Open a terminal and run: `python scrape_har_locations.py`
   - This will create:
     - An interactive map: `outputs/ip_map.html`
     - A GeoJSON file: `outputs/ip_locations.geojson`

## What to Submit

- **Screenshot:** Check out `webmap-screenshot.png` for a preview of the map you’ll create.
- **GeoJSON:** The script generates `outputs/ip_locations.geojson` with all the geolocated IPs.
- **Web Map Files:**
  - The main file is `custom_map.html` (or `index.html` if you rename it).
  - **Heads up:** The HTML file is self-contained—everything (CSS and JavaScript) is right inside. To view the map, just download the folder, open the HTML file in your browser, and make sure the `outputs/ip_locations.geojson` file is in the right spot. No extra CSS or JS files needed!

## What’s in This Folder?

- `scrape_har_locations.py` — The Python script that does all the work
- `custom_map.html` — The interactive web map (just open in your browser)
- `outputs/ip_locations.geojson` — The GeoJSON data for the map
- `webmap-screenshot.png` — A screenshot of the map
- `inputs/` — Where you put your HAR file

---
If you have any questions or run into any issues, feel free to reach out. Happy mapping!