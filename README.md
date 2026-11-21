# 🧭 Travel Planner & Explorer

Interactive, browser-native road trip exploration and getaway planning tools with 3D map visualization, dynamic road routing, elevation profiles, and AI-powered day itineraries.

Both applications run **100% standalone in your browser** with zero installation, zero server dependencies, and zero paid API keys required.

---

## 🚀 Included Applications

### 1. 🏞️ Weekend & Day Trip Explorer (`weekend_planner.html`)
Discover road trips, scenic viewpoints, waterfalls, ancient forts, temples, lakes, and wildlife sanctuaries within driving distance of any city.

* **Smart Radius & Time Filters**: Filter by **driving duration** (1 to 8 hours) or **distance** (50 to 500 km) with instant chips and fine-tuning sliders.
* **Category Filters**:
  * 🏰 Forts & Castles
  * 🌊 Waterfalls & Rivers
  * 🌄 Viewpoints & Hills
  * 🛕 Temples & Heritage
  * 🏞️ Lakes & Nature
  * 🦁 Wildlife & National Parks
  * 🌟 Top Attractions
* **High-Speed Batch Routing (OSRM Table API)**: Calculates exact driving distance and time for all candidate destinations in a single request.
* **Rich Destination Cards**: Automatically enriches places with Wikipedia thumbnail photos, descriptions, and one-tap Google Maps directions.
* **✨ AI Day Trip Planner**:
  * **Built-in Smart Heuristic Planner**: Works instantly offline with zero keys. Crafts realistic departure schedules, breakfast/lunch pitstops, sightseeing highlights, sunset points, packing checklists, and seasonal recommendations.
  * **Claude 3.5 & Gemini Support**: Optional setting to paste an Anthropic or Google Gemini API key (saved exclusively in browser `localStorage`) for custom AI-written plans.
* **Interactive Dark Map (Leaflet & Carto Dark Matter)**: Interactive coverage radius ring, pulsing origin pin, category-coded badges, and fly-to camera controls.

---

### 2. 🗺️ 3D Road Trip Visualizer (`Mahbubnagar to Indore trip map (worker test).html`)
A cinematic 3D globe visualization of the 866 km road journey from Mahbubnagar to Indore.

* **MapLibre 3D Globe**: Smooth 3D terrain and vector road geometry.
* **Dynamic From / To Route Search**:
  * Real-time geocoding autocomplete with Photon / OpenStreetMap.
  * 1-click direction swap (**`⇅`**) and origin/destination reversal.
  * Live route recalculation via OSRM driving engine.
  * 1-click **Default** button to restore the original 7-stop itinerary.
* **Dynamic Elevation Profile**: Real-time DEM elevation sampling along the highway route with peak altitude, elevation gain, and distance markers.
* **Responsive HUD Rail**: Itinerary breakdown, driving duration, distance statistics, and direct Google Maps navigation link.

---

## 💻 How to Run

No build step, Node.js, or server setup is required.

Simply open either file directly in any modern browser:
* Double-click `weekend_planner.html`
* Double-click `Mahbubnagar to Indore trip map (worker test).html`

Or serve locally with any static HTTP server:
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000/weekend_planner.html` in your browser.

---

## 🛠️ APIs & Open Data
* **Geocoding**: [Photon OpenStreetMap Geocoder](https://photon.komoot.io)
* **Road Routing**: [Project OSRM Driving Engine](https://project-osrm.org)
* **Elevation Data**: [Open-Meteo Elevation API](https://open-meteo.com)
* **Photos & Knowledge**: [Wikimedia / Wikipedia REST API](https://www.mediawiki.org/wiki/API:REST_API)
* **Map Tiles**: [Carto Dark Matter](https://carto.com/basemaps/) & [OpenStreetMap](https://www.openstreetmap.org)
