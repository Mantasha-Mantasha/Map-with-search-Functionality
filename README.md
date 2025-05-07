# Map with Search Functionality

This project demonstrates how to create an interactive map with search functionality using [Leaflet.js](https://leafletjs.com/) and the [Leaflet Control Geocoder plugin](https://github.com/perliedman/leaflet-control-geocoder).

## Features

- **Interactive Map**: Displays an interactive map centered on a specified location.
- **Search Functionality**: Allows users to search for locations using the Leaflet Control Geocoder.
- **OpenStreetMap Tiles**: Uses OpenStreetMap tiles for map rendering.
- **Geocoding Results**:
  - Adds a marker at the searched location.
  - Displays a popup with the location name.
  - Adjusts the map view to fit the bounding box of the searched location.

## How It Works

1. **Initialize the Map**:
   - The map is initialized with a center point at `[51.505, -0.09]` and a zoom level of `13`.

2. **Add OpenStreetMap Tiles**:
   - OpenStreetMap tiles are added to the map for rendering.

3. **Search Control**:
   - The search control is created using the Leaflet Control Geocoder plugin.
   - When a location is searched:
     - A bounding box is drawn around the location.
     - A marker is placed at the center of the location.
     - A popup displays the name of the location.
     - The map view adjusts to fit the bounding box.

## Usage

1. Include the required styles and scripts:
   - Leaflet CSS and JavaScript.
   - Leaflet Control Geocoder JavaScript.

2. Add a `<div>` element with the ID `map` to host the map.

3. Use the provided JavaScript code to:
   - Initialize the map.
   - Add OpenStreetMap tiles.
   - Configure the geocoder for search functionality.

4. Open the HTML file in a browser to view the map and use the search functionality.

## Prerequisites

- A modern web browser that supports JavaScript.
- Internet connection to load external libraries and map tiles from OpenStreetMap.

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/map-with-search.git
   cd map-with-search
   ```

2. Open the `index.html` file in your browser.

## Libraries Used

- [Leaflet.js](https://leafletjs.com/): A lightweight JavaScript library for interactive maps.
- [Leaflet Control Geocoder](https://github.com/perliedman/leaflet-control-geocoder): A plugin for adding geocoding functionality to Leaflet maps.
- [OpenStreetMap](https://www.openstreetmap.org/): Provides the map tiles used in this project.

## Customization

- **Default Center and Zoom**: Change the `setView` parameters to update the default map center and zoom level.
- **Map Tiles**: Replace the OpenStreetMap tile URL with a different tile provider if needed.
- **Search Control Options**: Customize the geocoder options in `L.Control.geocoder()` to fit specific requirements.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- Thanks to the contributors of [Leaflet.js](https://leafletjs.com/) and [Leaflet Control Geocoder](https://github.com/perliedman/leaflet-control-geocoder) for providing these powerful tools.
