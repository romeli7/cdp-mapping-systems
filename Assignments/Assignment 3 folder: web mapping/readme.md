# Geolocate HAR file IPs

This project extracts IP addresses from a HAR file, geolocates them using the ipinfo.io API, and visualizes their locations on an interactive web map using Folium and Leaflet.

## Usage

1. **Install required libraries:**
   - Make sure you have Python 3 and install dependencies with `pip install -r requirements.txt` (see `requirements.txt` for details).
2. **Prepare your HAR file:**
   - Download a HAR file from your browser and update the `HAR_FILE` variable in `scrape_har_locations.py`.
3. **Run the script:**
   - Execute: `python scrape_har_locations.py`
   - This will generate:
     - An interactive map: `outputs/ip_map.html`
     - A GeoJSON file: `outputs/ip_locations.geojson`

## Submission Instructions

- **Screenshot:** See `webmap-screenshot.png` for a preview of the web map.
- **GeoJSON:** The generated file is `outputs/ip_locations.geojson`.
- **Web Map Files:**
  - The main web map file is `custom_map.html` (or `index.html` if renamed).
  - **Note:** The HTML file is self-contained—all CSS and JavaScript are included within the file. To view the map, simply download the folder, open the HTML file in your browser, and ensure the `outputs/ip_locations.geojson` file is present in the correct location.
  - No separate CSS or JS files are needed.

## Folder Structure

- `scrape_har_locations.py` — Python script to extract and geolocate IPs
- `custom_map.html` — Self-contained web map (open in browser)
- `outputs/ip_locations.geojson` — GeoJSON data for the map
- `webmap-screenshot.png` — Screenshot of the web map
- `inputs/` — Place your HAR file here

---
If you have any questions or issues, please contact the project author.