# BusinessWA - Location Intelligence Dashboard

BusinessWA is a powerful location intelligence tool designed to help users analyze demographic and commercial data across Western Australia. By leveraging isochrone mapping (drive-time polygons), it provides actionable insights for business planning, site selection, and market analysis.

## Features

### 🗺️ Interactive Mapping
- **Dynamic Isochrones**: Visualize 3, 5, 7, and 10-minute drive-time areas from any location.
- **Search Functionality**: Instantly search for addresses, neighborhoods, or places of interest using the integrated Mapbox Geocoder.
- **POI Visualization**: View individual businesses on the map, color-coded by category (Retail, Food & Drink, Commercial).

### 📊 Data Analysis
- **Demographics**: Access population estimates, household density, age distribution, and gender breakdowns for the selected area.
- **Commercial Insights**: Analyze business counts, view top 10 businesses, and filter by category.
- **Zone Scoring**: Get a calculated "Zone Score" based on the area's vitality and density.

### ⚖️ Compare Mode
- **Split-Screen View**: Compare two locations side-by-side to evaluate their potential.
- **Comparison Matrix**: A dynamic grid highlights the "better" location for key metrics like population, business count, and median age.
- **Dual Controls**: Independent search bars and isochrone sliders for each map allow for flexible scenario testing.

## Tech Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Mapping**: [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/api/)
- **Geospatial Analysis**: [Turf.js](https://turfjs.org/)
- **Visualization**: [Chart.js](https://www.chartjs.org/)
- **Fonts**: Google Fonts (Inter)

## Getting Started

### Prerequisites
You will need a Mapbox Access Token. Replace the token in `index.html` with your own if you plan to deploy or use heavily.

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/nelsonucv/BusinessWA.git
   cd BusinessWA
   ```

2. **Run a local server**
   Since this project uses ES modules and CORS-restricted resources, it must be served via a local HTTP server (not just opening the file).

   Using Python:
   ```bash
   python3 -m http.server 8080
   ```

   Using Node.js (http-server):
   ```bash
   npx http-server .
   ```

3. **Open in Browser**
   Navigate to `http://localhost:8080` (or the port specified by your server).

## Version History

- **v1.0-prototype**: Initial release with functional dashboard, compare mode, and mock data integration.

## License

This project is open source.
