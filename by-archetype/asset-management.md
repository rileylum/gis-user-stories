# Asset Management Archetype

Track and manage physical assets with geographic locations.

## Archetype Overview

| Attribute | Description |
|-----------|-------------|
| **Primary Users** | Contributor, Analyst, Field Worker, Administrator |
| **Key Goal** | Maintain accurate records of physical assets |
| **Access Model** | Authenticated users with role-based permissions |
| **Editing** | Create, update, and manage asset records |
| **Examples** | Utility infrastructure, fleet tracking, property management, equipment inventory |

## Characteristics

- **CRUD operations**: Create, read, update, delete asset records
- **Rich attribute data**: Detailed asset properties and history
- **Workflow integration**: Often connected to work orders, inspections
- **Audit trail**: Track who changed what and when
- **Search and filter**: Find specific assets quickly
- **Multi-user**: Different roles (viewer, editor, admin)
- **Data quality**: Accurate, up-to-date information is critical

## Core Stories (Must Have)

These stories are essential for asset management:

### Navigation
- [NAV-001](../by-category/01-navigation.md#nav-001-pan-the-map): Pan the Map
- [NAV-002](../by-category/01-navigation.md#nav-002-zoom-with-mouse-wheel): Zoom with Mouse Wheel
- [NAV-006](../by-category/01-navigation.md#nav-006-reset-view): Reset View

### Display
- [DIS-001](../by-category/03-data-display.md#dis-001-display-basemap): Display Basemap
- [DIS-003](../by-category/03-data-display.md#dis-003-display-vector-features): Display Vector Features

### Layer Management
- [LAY-001](../by-category/02-layer-management.md#lay-001-toggle-layer-visibility): Toggle Layer Visibility

### Feature Interaction
- [INT-001](../by-category/04-feature-interaction.md#int-001-click-to-select-feature): Click to Select Feature
- [INT-004](../by-category/04-feature-interaction.md#int-004-display-feature-popup): Display Feature Popup
- [INT-005](../by-category/04-feature-interaction.md#int-005-filter-features-by-attribute): Filter Features by Attribute

### Drawing & Editing
- [DRW-001](../by-category/05-drawing-editing.md#drw-001-draw-point-feature): Draw Point Feature
- [DRW-006](../by-category/05-drawing-editing.md#drw-006-edit-feature-geometry): Edit Feature Geometry
- [DRW-007](../by-category/05-drawing-editing.md#drw-007-move-feature): Move Feature
- [DRW-008](../by-category/05-drawing-editing.md#drw-008-delete-feature): Delete Feature

### Search
- [SRC-001](../by-category/08-search-geocoding.md#src-001-search-by-addressplace): Search by Address/Place

### Controls
- [CTL-001](../by-category/09-controls-ui.md#ctl-001-display-zoom-buttons): Display Zoom Buttons
- [CTL-004](../by-category/09-controls-ui.md#ctl-004-display-attribution): Display Attribution

### Integration
- [ITG-003](../by-category/15-integration.md#itg-003-authenticate-users): Authenticate Users

### Administration
- [ADM-002](../by-category/16-administration.md#adm-002-manage-user-permissions): Manage User Permissions

### Error Handling
- [ERR-001](../by-category/18-error-handling.md#err-001-display-user-friendly-error-messages): User-Friendly Error Messages

## Recommended Stories (Should Have)

These stories significantly improve asset management workflows:

### Layer Management
- [LAY-002](../by-category/02-layer-management.md#lay-002-adjust-layer-opacity): Adjust Layer Opacity
- [LAY-003](../by-category/02-layer-management.md#lay-003-reorder-layers): Reorder Layers

### Display
- [DIS-002](../by-category/03-data-display.md#dis-002-switch-between-basemaps): Switch Between Basemaps
- [DIS-005](../by-category/03-data-display.md#dis-005-display-clustered-points): Display Clustered Points

### Feature Interaction
- [INT-002](../by-category/04-feature-interaction.md#int-002-box-select-multiple-features): Box Select Multiple Features
- [INT-003](../by-category/04-feature-interaction.md#int-003-hover-to-highlight-feature): Hover to Highlight Feature

### Drawing & Editing
- [DRW-002](../by-category/05-drawing-editing.md#drw-002-draw-line-feature): Draw Line Feature (for linear assets)
- [DRW-003](../by-category/05-drawing-editing.md#drw-003-draw-polygon-feature): Draw Polygon Feature (for area assets)
- [DRW-009](../by-category/05-drawing-editing.md#drw-009-snap-to-features): Snap to Features

### Search
- [SRC-002](../by-category/08-search-geocoding.md#src-002-search-by-coordinates): Search by Coordinates

### Styling
- [STY-001](../by-category/11-styling.md#sty-001-style-by-attribute-categorical): Style by Attribute (Categorical)
- [STY-002](../by-category/11-styling.md#sty-002-display-custom-iconssymbols): Display Custom Icons/Symbols
- [STY-003](../by-category/11-styling.md#sty-003-display-feature-labels): Display Feature Labels

### Data Management
- [DAT-001](../by-category/14-data-management.md#dat-001-upload-data): Upload Data
- [DAT-002](../by-category/14-data-management.md#dat-002-indicate-data-freshness): Indicate Data Freshness
- [DAT-003](../by-category/14-data-management.md#dat-003-download-data): Download Data

### Administration
- [ADM-001](../by-category/16-administration.md#adm-001-configure-layer-settings): Configure Layer Settings
- [ADM-004](../by-category/16-administration.md#adm-004-set-default-map-configuration): Set Default Map Configuration

### Performance
- [PRF-001](../by-category/17-performance.md#prf-001-fast-initial-load): Fast Initial Load
- [PRF-003](../by-category/17-performance.md#prf-003-display-loading-indicators): Display Loading Indicators

### Error Handling
- [ERR-002](../by-category/18-error-handling.md#err-002-retry-failed-operations): Retry Failed Operations

## Optional Stories (Nice to Have)

These stories add advanced capabilities:

### Display
- [DIS-004](../by-category/03-data-display.md#dis-004-display-heatmap): Display Heatmap (for density analysis)
- [DIS-007](../by-category/03-data-display.md#dis-007-display-temporal-data): Display Temporal Data

### Drawing
- [DRW-004](../by-category/05-drawing-editing.md#drw-004-draw-circle-feature): Draw Circle Feature

### Measurement
- [MEA-001](../by-category/06-measurement.md#mea-001-measure-distance): Measure Distance
- [MEA-002](../by-category/06-measurement.md#mea-002-measure-area): Measure Area

### Location
- [LOC-001](../by-category/07-location-services.md#loc-001-show-my-location): Show My Location

### Controls
- [CTL-003](../by-category/09-controls-ui.md#ctl-003-display-coordinates): Display Coordinates

### Import/Export
- [IMP-001](../by-category/10-import-export.md#imp-001-import-data-file): Import Data File
- [IMP-003](../by-category/10-import-export.md#imp-003-export-map-as-image): Export Map as Image
- [IMP-004](../by-category/10-import-export.md#imp-004-export-map-as-pdf): Export Map as PDF
- [IMP-005](../by-category/10-import-export.md#imp-005-generate-permalinkshare-url): Generate Permalink

### Styling
- [STY-004](../by-category/11-styling.md#sty-004-apply-color-ramp-graduated): Apply Color Ramp (Graduated)

### Data Management
- [DAT-004](../by-category/14-data-management.md#dat-004-data-versioning): Data Versioning

### Integration
- [ITG-004](../by-category/15-integration.md#itg-004-access-via-api): Access via API

### Compliance
- [CMP-003](../by-category/19-compliance.md#cmp-003-data-governance): Data Governance

## Not Typically Needed

These stories may not be relevant for asset management:

- Public Portal features: Usually internal users only
- Offline capability: Unless field teams need it
- Temporal animation: Unless tracking asset changes over time

## Example Use Cases

### Utility Infrastructure
- Poles, transformers, pipes, valves
- Categorized symbology by asset type and status
- Link to work order system
- Maintenance history per asset

### Fleet Management
- Vehicle locations (real-time or last known)
- Assignment and status tracking
- Route history
- Integration with telematics

### Facility Management
- Building footprints with floor plans
- Equipment within buildings
- Maintenance schedules
- Space utilization

## Key Customization Questions

1. What types of assets will be managed?
2. What attributes need to be tracked for each asset type?
3. Who can create, edit, and delete assets?
4. Is there an integration with work order or ERP systems?
5. Is an audit trail required for compliance?
6. Do field workers need mobile/offline access?
7. What reports are needed?

## Related Starter Kit

See [Asset Management Starter Kit](../quick-start/starter-kits/asset-management-starter.md) for a copy-paste ready story set.
