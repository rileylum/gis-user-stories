# Analysis Tool Archetype

Spatial analysis and decision support applications.

## Archetype Overview

| Attribute | Description |
|-----------|-------------|
| **Primary Users** | Analyst, Viewer |
| **Key Goal** | Enable data-driven geographic decision making |
| **Access Model** | Authenticated, typically internal |
| **Editing** | Analysis outputs, not source data |
| **Examples** | Site selection, risk analysis, market research, resource planning |

## Characteristics

- **Data-rich**: Multiple layers of information
- **Query and filter**: Flexible data exploration
- **Visualization**: Thematic maps, charts, statistics
- **Measurement**: Distance, area, proximity
- **Comparison**: Before/after, scenario analysis
- **Export**: Reports, images, data downloads
- **Complex workflows**: Multi-step analysis processes
- **Precision**: Accurate coordinates and projections

## Core Stories (Must Have)

These stories are essential for analysis tools:

### Navigation
- [NAV-001](../by-category/01-navigation.md#nav-001-pan-the-map): Pan the Map
- [NAV-002](../by-category/01-navigation.md#nav-002-zoom-with-mouse-wheel): Zoom with Mouse Wheel
- [NAV-006](../by-category/01-navigation.md#nav-006-reset-view): Reset View

### Display
- [DIS-001](../by-category/03-data-display.md#dis-001-display-basemap): Display Basemap
- [DIS-002](../by-category/03-data-display.md#dis-002-switch-between-basemaps): Switch Between Basemaps
- [DIS-003](../by-category/03-data-display.md#dis-003-display-vector-features): Display Vector Features

### Layer Management
- [LAY-001](../by-category/02-layer-management.md#lay-001-toggle-layer-visibility): Toggle Layer Visibility
- [LAY-002](../by-category/02-layer-management.md#lay-002-adjust-layer-opacity): Adjust Layer Opacity
- [LAY-003](../by-category/02-layer-management.md#lay-003-reorder-layers): Reorder Layers

### Feature Interaction
- [INT-001](../by-category/04-feature-interaction.md#int-001-click-to-select-feature): Click to Select Feature
- [INT-002](../by-category/04-feature-interaction.md#int-002-box-select-multiple-features): Box Select Multiple Features
- [INT-003](../by-category/04-feature-interaction.md#int-003-hover-to-highlight-feature): Hover to Highlight Feature
- [INT-004](../by-category/04-feature-interaction.md#int-004-display-feature-popup): Display Feature Popup
- [INT-005](../by-category/04-feature-interaction.md#int-005-filter-features-by-attribute): Filter Features by Attribute

### Measurement
- [MEA-001](../by-category/06-measurement.md#mea-001-measure-distance): Measure Distance
- [MEA-002](../by-category/06-measurement.md#mea-002-measure-area): Measure Area

### Controls
- [CTL-001](../by-category/09-controls-ui.md#ctl-001-display-zoom-buttons): Display Zoom Buttons
- [CTL-002](../by-category/09-controls-ui.md#ctl-002-display-scale-bar): Display Scale Bar
- [CTL-003](../by-category/09-controls-ui.md#ctl-003-display-coordinates): Display Coordinates
- [CTL-004](../by-category/09-controls-ui.md#ctl-004-display-attribution): Display Attribution

### Styling
- [STY-001](../by-category/11-styling.md#sty-001-style-by-attribute-categorical): Style by Attribute (Categorical)
- [STY-004](../by-category/11-styling.md#sty-004-apply-color-ramp-graduated): Apply Color Ramp (Graduated)

### Integration
- [ITG-003](../by-category/15-integration.md#itg-003-authenticate-users): Authenticate Users

### Error Handling
- [ERR-001](../by-category/18-error-handling.md#err-001-display-user-friendly-error-messages): User-Friendly Error Messages

## Recommended Stories (Should Have)

These stories significantly enhance analysis capabilities:

### Navigation
- [NAV-003](../by-category/01-navigation.md#nav-003-zoom-with-double-clicktap): Zoom with Double-Click
- [NAV-005](../by-category/01-navigation.md#nav-005-rotate-the-map): Rotate the Map

### Display
- [DIS-004](../by-category/03-data-display.md#dis-004-display-heatmap): Display Heatmap
- [DIS-005](../by-category/03-data-display.md#dis-005-display-clustered-points): Display Clustered Points
- [DIS-006](../by-category/03-data-display.md#dis-006-display-graticulegrid): Display Graticule

### Layer Management
- [LAY-004](../by-category/02-layer-management.md#lay-004-compare-layers-with-swipesplit): Compare Layers (Swipe/Split)
- [LAY-005](../by-category/02-layer-management.md#lay-005-display-minimapoverview): Display Minimap

### Drawing (for analysis areas)
- [DRW-003](../by-category/05-drawing-editing.md#drw-003-draw-polygon-feature): Draw Polygon Feature
- [DRW-004](../by-category/05-drawing-editing.md#drw-004-draw-circle-feature): Draw Circle Feature (buffers)

### Measurement
- [MEA-003](../by-category/06-measurement.md#mea-003-live-measurement-display): Live Measurement Display

### Search
- [SRC-001](../by-category/08-search-geocoding.md#src-001-search-by-addressplace): Search by Address/Place
- [SRC-002](../by-category/08-search-geocoding.md#src-002-search-by-coordinates): Search by Coordinates
- [SRC-003](../by-category/08-search-geocoding.md#src-003-reverse-geocode-click-to-address): Reverse Geocode

### Controls
- [CTL-005](../by-category/09-controls-ui.md#ctl-005-fullscreen-mode): Fullscreen Mode

### Import/Export
- [IMP-001](../by-category/10-import-export.md#imp-001-import-data-file): Import Data File
- [IMP-003](../by-category/10-import-export.md#imp-003-export-map-as-image): Export Map as Image
- [IMP-004](../by-category/10-import-export.md#imp-004-export-map-as-pdf): Export Map as PDF
- [IMP-005](../by-category/10-import-export.md#imp-005-generate-permalinkshare-url): Generate Permalink

### Styling
- [STY-003](../by-category/11-styling.md#sty-003-display-feature-labels): Display Feature Labels

### Projections
- [PRJ-001](../by-category/12-projections.md#prj-001-display-coordinates-in-multiple-formats): Display Coordinates in Multiple Formats
- [PRJ-002](../by-category/12-projections.md#prj-002-transform-coordinates-between-systems): Transform Coordinates

### Data Management
- [DAT-002](../by-category/14-data-management.md#dat-002-indicate-data-freshness): Indicate Data Freshness
- [DAT-003](../by-category/14-data-management.md#dat-003-download-data): Download Data

### Geoprocessing
- [GPR-001](../by-category/22-geoprocessing.md#gpr-001-buffer-features): Buffer Features
- [GPR-002](../by-category/22-geoprocessing.md#gpr-002-intersectclip-layers): Intersect/Clip Layers
- [GPR-003](../by-category/22-geoprocessing.md#gpr-003-unionmerge-features): Union/Merge Features

### Charts
- [CHT-001](../by-category/24-charts-dashboards.md#cht-001-display-attribute-chart-bar-pie-line): Display Attribute Chart
- [CHT-003](../by-category/24-charts-dashboards.md#cht-003-display-summary-statistics-panel): Display Summary Statistics Panel

### Performance
- [PRF-001](../by-category/17-performance.md#prf-001-fast-initial-load): Fast Initial Load
- [PRF-003](../by-category/17-performance.md#prf-003-display-loading-indicators): Display Loading Indicators
- [PRF-004](../by-category/17-performance.md#prf-004-cache-data-efficiently): Cache Data Efficiently

## Optional Stories (Nice to Have)

These stories add advanced analysis capabilities:

### Display
- [DIS-007](../by-category/03-data-display.md#dis-007-display-temporal-data): Display Temporal Data

### Styling
- [STY-002](../by-category/11-styling.md#sty-002-display-custom-iconssymbols): Display Custom Icons

### Projections
- [PRJ-003](../by-category/12-projections.md#prj-003-display-map-in-different-projections): Display Map in Different Projections

### Import/Export
- [IMP-002](../by-category/10-import-export.md#imp-002-drag-and-drop-import): Drag and Drop Import

### Data Management
- [DAT-001](../by-category/14-data-management.md#dat-001-upload-data): Upload Data

### Integration
- [ITG-001](../by-category/15-integration.md#itg-001-share-map-view): Share Map View
- [ITG-004](../by-category/15-integration.md#itg-004-access-via-api): Access via API

### Administration
- [ADM-001](../by-category/16-administration.md#adm-001-configure-layer-settings): Configure Layer Settings
- [ADM-004](../by-category/16-administration.md#adm-004-set-default-map-configuration): Set Default Map Configuration

### Accessibility
- [ACC-001](../by-category/13-accessibility.md#acc-001-keyboard-navigation): Keyboard Navigation

### Compliance
- [CMP-003](../by-category/19-compliance.md#cmp-003-data-governance): Data Governance

### Geoprocessing (Advanced)
- [GPR-004](../by-category/22-geoprocessing.md#gpr-004-spatial-join-point-in-polygon-nearest): Spatial Join
- [GPR-005](../by-category/22-geoprocessing.md#gpr-005-calculate-statistics-by-area): Calculate Statistics by Area

### Routing
- [RTE-005](../by-category/20-routing.md#rte-005-calculate-service-areasisochrones): Calculate Service Areas/Isochrones

### Charts (Advanced)
- [CHT-002](../by-category/24-charts-dashboards.md#cht-002-link-chart-to-map-selection): Link Chart to Map Selection
- [CHT-004](../by-category/24-charts-dashboards.md#cht-004-create-dashboard-layout): Create Dashboard Layout

### 3D & Terrain
- [3DT-001](../by-category/25-3d-terrain.md#3dt-001-display-3d-terrainelevation): Display 3D Terrain
- [3DT-002](../by-category/25-3d-terrain.md#3dt-002-extrude-features-by-attribute): Extrude Features by Attribute

## Not Typically Needed

These stories may not be relevant for analysis tools:

- Offline capability: Analysis usually done at a workstation
- Location services: Not field-based
- Field-oriented editing workflows

## Example Use Cases

### Site Selection
- Overlay multiple criteria layers
- Buffer around existing facilities
- Score and rank candidate locations
- Compare scenarios
- Export shortlist with supporting data

### Risk Assessment
- Visualize hazard zones
- Query at-risk assets
- Generate exposure statistics
- Create risk maps for reports
- Historical comparison

### Market Analysis
- Demographic data visualization
- Trade area analysis
- Competitor proximity
- Drive-time polygons
- Export market reports

### Resource Planning
- Service area coverage
- Gap analysis
- Demand forecasting
- Scenario comparison
- Report generation

## Key Customization Questions

1. What types of analysis will users perform?
2. What data layers are needed?
3. What geoprocessing operations are required?
4. What reports or exports are needed?
5. Should users be able to save analysis sessions?
6. Is temporal analysis (change over time) needed?
7. What level of coordinate precision is required?
8. Are there specific projection requirements?

## Related Resources

Analysis tools often combine multiple starter kits. See:
- [MVP Checklist](../quick-start/mvp-checklist.md) for foundation stories
- [Dependency Graph](../dependencies/dependency-graph.md) for story relationships
