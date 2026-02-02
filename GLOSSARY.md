# Web Mapping Glossary

A plain-language guide to GIS and web mapping terminology used throughout this repository.

---

## A

### Accuracy (GPS)
How close a GPS reading is to the actual location. Typically measured in meters. Consumer devices are usually accurate to 3-10 meters.

### Annotation
Text or symbols added to a map to provide additional information, such as labels or callouts.

### Attribution
Credit given to data providers and map sources. Often displayed in the corner of the map (e.g., "© OpenStreetMap contributors").

---

## B

### Basemap
The background map layer that provides geographic context. Examples include street maps, satellite imagery, and topographic maps.

### Bounding Box
A rectangular area defined by minimum and maximum coordinates (min X, min Y, max X, max Y). Used to specify the visible extent of a map.

### Buffer
A zone of a specified distance around a feature. For example, a 500-meter buffer around a school.

---

## C

### Centroid
The geometric center point of a shape. Used for placing labels or as a reference point.

### Cluster
A group of nearby point features combined into a single symbol to reduce visual clutter. Common for maps with many markers.

### Coordinate
A pair of numbers (X, Y) or (longitude, latitude) that specify a location on Earth.

### CRS (Coordinate Reference System)
See "Projection."

---

## D

### Datum
A reference model of Earth's shape used for mapping. Common datums include WGS84 (used by GPS) and NAD83 (used in North America).

### Digitizing
The process of creating digital map features by tracing or drawing on a map.

---

## E

### Extent
The geographic area visible in the current map view. Defined by the bounding coordinates.

### EPSG Code
A standardized numeric code identifying a coordinate reference system. Examples:
- EPSG:4326 = WGS84 (lat/lon in degrees)
- EPSG:3857 = Web Mercator (meters, used by web maps)

---

## F

### Feature
A geographic object on a map, such as a point (city), line (road), or polygon (park).

### Feature Class
A collection of features of the same geometry type with the same attributes.

---

## G

### Geocoding
Converting an address or place name into geographic coordinates. Example: "123 Main St" → (40.7128, -74.0060).

### Geodetic
Relating to the measurement of Earth's shape and size. Geodetic calculations account for Earth's curvature.

### GeoJSON
A popular format for encoding geographic features using JSON. Easy to read and widely supported by web mapping libraries.

### Geometry
The shape of a geographic feature: point, line (or polyline), polygon, or collections of these.

### Geolocation
Determining the geographic position of a device, typically using GPS or network-based methods.

### Geoprocessing
Operations that analyze or transform geographic data, such as buffering, intersecting, or dissolving features.

### GIS (Geographic Information System)
Software and methods for capturing, storing, analyzing, and displaying geographic data.

### Graticule
A network of latitude and longitude lines drawn on a map.

---

## H

### Heatmap
A visualization showing the density or intensity of point data using color gradients. Hot colors indicate high concentration.

### Hexbin
A grid of hexagonal cells used to aggregate point data for visualization.

---

## I

### Intersect
A spatial operation that finds areas where two features overlap.

---

## K

### KML (Keyhole Markup Language)
An XML format for geographic data, originally developed for Google Earth.

### Kinetic Scrolling
The "momentum" effect where a map continues to pan briefly after the user stops dragging.

---

## L

### Layer
A collection of geographic features displayed together on a map. Maps are built by stacking multiple layers.

### Legend
A key explaining the symbols and colors used on a map.

### Line String / Polyline
A geometry type representing a connected series of points forming a line.

---

## M

### Marker
A symbol (often a pin or dot) placed on a map to indicate a point location.

### Mercator Projection
A map projection that preserves angles and shapes at the cost of distorting size at high latitudes. Web Mercator is the standard for web maps.

### Metadata
Information about data, such as creation date, source, accuracy, and coordinate system.

### Minimap
A small overview map showing the current view's position within a larger area.

---

## N

### Node
A single coordinate point. Lines and polygons are made up of connected nodes.

---

## O

### OGC (Open Geospatial Consortium)
An organization that develops standards for geospatial data and services (WMS, WFS, WCS, etc.).

### Opacity
The transparency level of a layer, from 0% (invisible) to 100% (fully opaque).

### Overlay
A layer displayed on top of the basemap.

---

## P

### Pan
Moving the map view by dragging to see different areas.

### Point
A geometry type representing a single location (X, Y coordinates).

### Polygon
A geometry type representing a closed shape with an interior area.

### Popup
An information bubble that appears when clicking or hovering over a map feature.

### Projection
A mathematical method for displaying Earth's curved surface on a flat map. Different projections preserve different properties (area, shape, distance, direction).

---

## R

### Raster
Geographic data stored as a grid of cells (pixels), such as satellite imagery or elevation data.

### Reverse Geocoding
Converting coordinates into an address or place name. The opposite of geocoding.

---

## S

### Scale
The ratio between distance on the map and distance in the real world. A scale of 1:10,000 means 1 cm on the map equals 10,000 cm (100 m) in reality.

### Scale Bar
A visual indicator on the map showing distance at the current zoom level.

### Shapefile
A common vector data format developed by Esri. Consists of multiple files (.shp, .shx, .dbf, etc.).

### Snap / Snapping
Automatically aligning new geometry to existing features, such as snapping a new road segment to an intersection.

### Spatial Query
Finding features based on their location or relationship to other features (e.g., "find all restaurants within 1 km").

### Symbology
The visual representation of features on a map, including colors, shapes, and sizes.

---

## T

### Tile
A small, pre-rendered image (typically 256x256 pixels) used to display basemaps efficiently. Maps load tiles as needed based on zoom and extent.

### Topology
The spatial relationships between features, such as connectivity and adjacency.

---

## V

### Vector
Geographic data stored as coordinates defining points, lines, and polygons. Opposite of raster.

### Viewport
The visible area of the map on screen.

---

## W

### WCS (Web Coverage Service)
An OGC standard for serving raster data (like satellite imagery) over the web.

### WFS (Web Feature Service)
An OGC standard for serving vector data (features) over the web. Allows querying and editing.

### WGS84
The World Geodetic System 1984. The coordinate system used by GPS, with coordinates in degrees of latitude and longitude.

### WMS (Web Map Service)
An OGC standard for serving pre-rendered map images over the web.

### WMTS (Web Map Tile Service)
An OGC standard for serving pre-rendered map tiles.

---

## X

### XYZ Tiles
A common tile scheme where tiles are addressed by zoom level (Z), column (X), and row (Y).

---

## Z

### Zoom
Changing the map scale to see more or less area. Zooming in shows more detail; zooming out shows more area.

### Zoom Level
A discrete scale level in a tiled map. Level 0 shows the whole world; each level doubles the resolution. Web maps typically have zoom levels 0-20.
