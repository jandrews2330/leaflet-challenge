# leaflet-challenge
This project is an interactive web map that visualizes real-time earthquake data from the USGS using [Leaflet.js](https://leafletjs.com/) and [D3.js](https://d3js.org/). Users can explore earthquake locations, magnitudes, depths, and see tectonic plate boundaries as overlays.

## How This Dashboard Was Built

1. **Project Setup**
    - Directory was pre-populated in starter code with the `static/js`, `static/css`, and `index.html`

2. **Map Initialization**
    - Used Leaflet to create a map centered on `[37.09, -95.71]` (central US).
    - Added OpenStreetMap tiles as the default base layer, and a 'Streets' layer as an option.
    - Added LayerGroups for earthquakes and tectonic plates, plus a layer control UI.

3. **Loading and Visualizing Earthquake Data**
    - Used D3 to load USGS GeoJSON earthquake data (all earthquakes from the past 7 days).
    - Created a function to style markers by depth (color) and magnitude (size).
    - Plotted earthquakes as circle markers with interactive popups.
    - Added the earthquakes as a toggleable overlay.

4. **Legend and Interactivity**
    - Built a map legend for depth color-coding using Leaflet’s control features.
    - Added popups for all earthquake markers, displaying relevant information.

5. **Tectonic Plate Overlay**
    - Used D3 to load tectonic plate boundaries GeoJSON from GitHub.
    - Displayed plate boundaries as orange lines, toggleable via the map control.

6. **Deployment**
    - Pushed files to GitHub and deployed as a static site using GitHub Pages.

---

## How to Use

- Open `index.html` in your browser (or visit (https://jandrews2330.github.io/leaflet-challenge/)).
- Use the layer control (top right) to toggle between base maps and overlays.
- Click any circle marker to view earthquake details.
- Reference the legend (bottom right) for color coding by depth.

## Credits

- Visualizations were created using the provided examples in the assignment, referencing prior class examples, and the assistance of Xpert Learning Assistance. 
- Earthquake data courtesy of [USGS Earthquake Hazards Program](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php).
- Tectonic plate boundaries courtesy of [Fraxen on GitHub](https://github.com/fraxen/tectonicplates).
- Map tiles by [OpenStreetMap](https://www.openstreetmap.org/).