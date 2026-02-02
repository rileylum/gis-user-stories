# Data Viewer Archetype

Internal data visualization applications for exploring and understanding geographic data.

## Archetype Overview

| Attribute | Description |
|-----------|-------------|
| **Primary Users** | Viewer, Analyst |
| **Key Goal** | Enable exploration and understanding of organizational data |
| **Access Model** | Authenticated, internal users |
| **Editing** | Read-only; view and query only |
| **Examples** | Business intelligence dashboards, data exploration, reporting tools |

## Characteristics

- **Read-only**: No editing, focused on viewing and querying
- **Multiple data sources**: Combine various layers and datasets
- **Visualization options**: Different ways to display the same data
- **Query and filter**: Find and highlight specific information
- **Dashboard integration**: Often part of larger BI platform
- **Export capability**: Share findings as images or data
- **Performance focused**: Handle large datasets smoothly
- **Accessible**: Available to many internal users

## Core Stories (Must Have)

These stories are essential for data viewers:

### Navigation
- [NAV-001](../by-category/01-navigation.md#nav-001-pan-the-map): Pan the Map
- [NAV-002](../by-category/01-navigation.md#nav-002-zoom-with-mouse-wheel): Zoom with Mouse Wheel
- [NAV-003](../by-category/01-navigation.md#nav-003-zoom-with-double-clicktap): Zoom with Double-Click
- [NAV-006](../by-category/01-navigation.md#nav-006-reset-view): Reset View

### Display
- [DIS-001](../by-category/03-data-display.md#dis-001-display-basemap): Display Basemap
- [DIS-003](../by-category/03-data-display.md#dis-003-display-vector-features): Display Vector Features

### Layer Management
- [LAY-001](../by-category/02-layer-management.md#lay-001-toggle-layer-visibility): Toggle Layer Visibility
- [LAY-002](../by-category/02-layer-management.md#lay-002-adjust-layer-opacity): Adjust Layer Opacity

### Feature Interaction
- [INT-001](../by-category/04-feature-interaction.md#int-001-click-to-select-feature): Click to Select Feature
- [INT-003](../by-category/04-feature-interaction.md#int-003-hover-to-highlight-feature): Hover to Highlight Feature
- [INT-004](../by-category/04-feature-interaction.md#int-004-display-feature-popup): Display Feature Popup
- [INT-005](../by-category/04-feature-interaction.md#int-005-filter-features-by-attribute): Filter Features by Attribute

### Controls
- [CTL-001](../by-category/09-controls-ui.md#ctl-001-display-zoom-buttons): Display Zoom Buttons
- [CTL-002](../by-category/09-controls-ui.md#ctl-002-display-scale-bar): Display Scale Bar
- [CTL-004](../by-category/09-controls-ui.md#ctl-004-display-attribution): Display Attribution

### Styling
- [STY-001](../by-category/11-styling.md#sty-001-style-by-attribute-categorical): Style by Attribute (Categorical)

### Controls
- [CTL-007](../by-category/09-controls-ui.md#ctl-007-display-legend): Display Legend

### Integration
- [ITG-003](../by-category/15-integration.md#itg-003-authenticate-users): Authenticate Users

### Performance
- [PRF-001](../by-category/17-performance.md#prf-001-fast-initial-load): Fast Initial Load
- [PRF-003](../by-category/17-performance.md#prf-003-display-loading-indicators): Display Loading Indicators

### Error Handling
- [ERR-001](../by-category/18-error-handling.md#err-001-display-user-friendly-error-messages): User-Friendly Error Messages

## Recommended Stories (Should Have)

These stories significantly enhance the viewing experience:

### Navigation
- [NAV-004](../by-category/01-navigation.md#nav-004-zoom-with-pinch-gesture): Zoom with Pinch Gesture
- [NAV-007](../by-category/01-navigation.md#nav-007-kinetic-panning-momentum): Kinetic Panning

### Display
- [DIS-002](../by-category/03-data-display.md#dis-002-switch-between-basemaps): Switch Between Basemaps
- [DIS-004](../by-category/03-data-display.md#dis-004-display-heatmap): Display Heatmap
- [DIS-005](../by-category/03-data-display.md#dis-005-display-clustered-points): Display Clustered Points

### Layer Management
- [LAY-003](../by-category/02-layer-management.md#lay-003-reorder-layers): Reorder Layers
- [LAY-004](../by-category/02-layer-management.md#lay-004-compare-layers-with-swipesplit): Compare Layers
- [LAY-005](../by-category/02-layer-management.md#lay-005-display-minimapoverview): Display Minimap

### Feature Interaction
- [INT-002](../by-category/04-feature-interaction.md#int-002-box-select-multiple-features): Box Select Multiple Features

### Search
- [SRC-001](../by-category/08-search-geocoding.md#src-001-search-by-addressplace): Search by Address/Place

### Controls
- [CTL-005](../by-category/09-controls-ui.md#ctl-005-fullscreen-mode): Fullscreen Mode

### Navigation
- [NAV-008](../by-category/01-navigation.md#nav-008-save-and-restore-map-views-bookmarks): Save and Restore Map Views (Bookmarks)

### Import/Export
- [IMP-003](../by-category/10-import-export.md#imp-003-export-map-as-image): Export Map as Image
- [IMP-005](../by-category/10-import-export.md#imp-005-generate-permalinkshare-url): Generate Permalink

### Styling
- [STY-003](../by-category/11-styling.md#sty-003-display-feature-labels): Display Feature Labels
- [STY-004](../by-category/11-styling.md#sty-004-apply-color-ramp-graduated): Apply Color Ramp

### Data Management
- [DAT-002](../by-category/14-data-management.md#dat-002-indicate-data-freshness): Indicate Data Freshness

### Integration
- [ITG-001](../by-category/15-integration.md#itg-001-share-map-view): Share Map View

### Performance
- [PRF-004](../by-category/17-performance.md#prf-004-cache-data-efficiently): Cache Data Efficiently

### Accessibility
- [ACC-001](../by-category/13-accessibility.md#acc-001-keyboard-navigation): Keyboard Navigation

## Optional Stories (Nice to Have)

These stories add advanced visualization capabilities:

### Display
- [DIS-006](../by-category/03-data-display.md#dis-006-display-graticulegrid): Display Graticule
- [DIS-007](../by-category/03-data-display.md#dis-007-display-temporal-data): Display Temporal Data

### Search
- [SRC-002](../by-category/08-search-geocoding.md#src-002-search-by-coordinates): Search by Coordinates

### Controls
- [CTL-003](../by-category/09-controls-ui.md#ctl-003-display-coordinates): Display Coordinates

### Import/Export
- [IMP-001](../by-category/10-import-export.md#imp-001-import-data-file): Import Data File
- [IMP-004](../by-category/10-import-export.md#imp-004-export-map-as-pdf): Export Map as PDF

### Styling
- [STY-002](../by-category/11-styling.md#sty-002-display-custom-iconssymbols): Display Custom Icons

### Data Management
- [DAT-003](../by-category/14-data-management.md#dat-003-download-data): Download Data

### Integration
- [ITG-002](../by-category/15-integration.md#itg-002-embed-map-in-website): Embed Map in Website

### Administration
- [ADM-001](../by-category/16-administration.md#adm-001-configure-layer-settings): Configure Layer Settings
- [ADM-004](../by-category/16-administration.md#adm-004-set-default-map-configuration): Set Default Map Configuration

### Accessibility
- [ACC-002](../by-category/13-accessibility.md#acc-002-screen-reader-support): Screen Reader Support
- [ACC-003](../by-category/13-accessibility.md#acc-003-high-contrast-mode): High Contrast Mode

## Not Typically Needed

These stories are usually not applicable to data viewers:

- Drawing & Editing (DRW-*): Read-only application
- Location Services (LOC-*): Not field-based
- Offline capability: Desktop/web application
- Measurement tools: Unless specifically needed
- Data upload/versioning: Managed elsewhere

## Example Use Cases

### Executive Dashboard
- High-level geographic KPIs
- Regional performance comparison
- Drill-down to details
- Shareable views
- Clean, simple interface

### Sales Territory View
- Territory boundaries and assignments
- Performance by region
- Customer locations
- Opportunity visualization
- Filter by product/time period

### Inventory Visualization
- Warehouse and store locations
- Stock levels by location
- Supply chain visualization
- Real-time updates
- Alert indicators

### Demographic Explorer
- Census and demographic data
- Thematic mapping by variable
- Compare multiple variables
- Area selection for statistics
- Export data for further analysis

## Key Customization Questions

1. What data will be visualized?
2. Who are the primary users (executives, analysts, all staff)?
3. Will this integrate with existing BI tools?
4. What filtering and query capabilities are needed?
5. What export formats are required?
6. Is real-time data refresh needed?
7. Should views be shareable/bookmarkable?
8. What performance is expected (number of features, load time)?

## Related Resources

Data viewers share many stories with public portals but require authentication. See:
- [Public Portal Archetype](public-portal.md) for comparison
- [Analysis Tool Archetype](analysis-tool.md) for more advanced analysis needs
- [MVP Checklist](../quick-start/mvp-checklist.md) for foundation stories
