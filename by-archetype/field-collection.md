# Field Collection Archetype

Mobile data gathering applications for field workers.

## Archetype Overview

| Attribute | Description |
|-----------|-------------|
| **Primary Users** | Field Worker, Contributor |
| **Key Goal** | Collect accurate data in the field efficiently |
| **Access Model** | Authenticated, often personal devices |
| **Editing** | Create and update records on location |
| **Examples** | Inspections, surveys, damage assessment, environmental monitoring |

## Characteristics

- **Mobile-first**: Designed primarily for phones and tablets
- **GPS-centric**: Leverage device location for placement accuracy
- **Offline-capable**: Must work in areas with poor connectivity
- **Form-based**: Structured data entry with validation
- **Photo/media capture**: Often includes photos attached to features
- **Sync and queue**: Handle intermittent connectivity gracefully
- **Battery-conscious**: Efficient use of GPS and network
- **Touch-optimized**: Large buttons, easy gestures

## Core Stories (Must Have)

These stories are essential for field collection:

### Navigation
- [NAV-001](../by-category/01-navigation.md#nav-001-pan-the-map): Pan the Map
- [NAV-004](../by-category/01-navigation.md#nav-004-zoom-with-pinch-gesture): Zoom with Pinch Gesture
- [NAV-006](../by-category/01-navigation.md#nav-006-reset-view): Reset View

### Display
- [DIS-001](../by-category/03-data-display.md#dis-001-display-basemap): Display Basemap
- [DIS-003](../by-category/03-data-display.md#dis-003-display-vector-features): Display Vector Features

### Layer Management
- [LAY-001](../by-category/02-layer-management.md#lay-001-toggle-layer-visibility): Toggle Layer Visibility

### Feature Interaction
- [INT-001](../by-category/04-feature-interaction.md#int-001-click-to-select-feature): Click to Select Feature
- [INT-004](../by-category/04-feature-interaction.md#int-004-display-feature-popup): Display Feature Popup

### Drawing & Editing
- [DRW-001](../by-category/05-drawing-editing.md#drw-001-draw-point-feature): Draw Point Feature
- [DRW-006](../by-category/05-drawing-editing.md#drw-006-edit-feature-geometry): Edit Feature Geometry
- [DRW-008](../by-category/05-drawing-editing.md#drw-008-delete-feature): Delete Feature
- [DRW-010](../by-category/05-drawing-editing.md#drw-010-undoredo-actions): Undo/Redo Actions

### Feature Interaction
- [INT-006](../by-category/04-feature-interaction.md#int-006-edit-feature-attributes): Edit Feature Attributes

### Location Services
- [LOC-001](../by-category/07-location-services.md#loc-001-show-my-location): Show My Location
- [LOC-003](../by-category/07-location-services.md#loc-003-center-map-on-my-location): Center Map on My Location
- [LOC-004](../by-category/07-location-services.md#loc-004-show-location-accuracy): Show Location Accuracy

### Controls
- [CTL-001](../by-category/09-controls-ui.md#ctl-001-display-zoom-buttons): Display Zoom Buttons

### Integration
- [ITG-003](../by-category/15-integration.md#itg-003-authenticate-users): Authenticate Users

### Error Handling
- [ERR-001](../by-category/18-error-handling.md#err-001-display-user-friendly-error-messages): User-Friendly Error Messages
- [ERR-003](../by-category/18-error-handling.md#err-003-auto-save-drafts): Auto-Save Drafts

### Performance (Critical for Field Work)
- [PRF-002](../by-category/17-performance.md#prf-002-offline-capability): Offline Capability

## Recommended Stories (Should Have)

These stories significantly improve field collection workflows:

### Navigation
- [NAV-003](../by-category/01-navigation.md#nav-003-zoom-with-double-clicktap): Zoom with Double-Click/Tap
- [NAV-005](../by-category/01-navigation.md#nav-005-rotate-the-map): Rotate the Map (for orientation)
- [NAV-007](../by-category/01-navigation.md#nav-007-kinetic-panning-momentum): Kinetic Panning

### Display
- [DIS-002](../by-category/03-data-display.md#dis-002-switch-between-basemaps): Switch Between Basemaps

### Drawing & Editing
- [DRW-002](../by-category/05-drawing-editing.md#drw-002-draw-line-feature): Draw Line Feature
- [DRW-003](../by-category/05-drawing-editing.md#drw-003-draw-polygon-feature): Draw Polygon Feature
- [DRW-005](../by-category/05-drawing-editing.md#drw-005-freehand-drawing): Freehand Drawing
- [DRW-007](../by-category/05-drawing-editing.md#drw-007-move-feature): Move Feature
- [DRW-009](../by-category/05-drawing-editing.md#drw-009-snap-to-features): Snap to Features

### Location Services
- [LOC-002](../by-category/07-location-services.md#loc-002-track-my-location): Track My Location

### Search
- [SRC-001](../by-category/08-search-geocoding.md#src-001-search-by-addressplace): Search by Address/Place
- [SRC-003](../by-category/08-search-geocoding.md#src-003-reverse-geocode-click-to-address): Reverse Geocode

### Routing
- [RTE-001](../by-category/20-routing.md#rte-001-calculate-route-between-points): Calculate Route Between Points
- [RTE-002](../by-category/20-routing.md#rte-002-display-turn-by-turn-directions): Display Turn-by-Turn Directions

### Controls
- [CTL-006](../by-category/09-controls-ui.md#ctl-006-display-compassnorth-arrow): Display Compass

### Styling
- [STY-002](../by-category/11-styling.md#sty-002-display-custom-iconssymbols): Display Custom Icons/Symbols

### Accessibility
- [ACC-001](../by-category/13-accessibility.md#acc-001-keyboard-navigation): Keyboard Navigation

### Performance
- [PRF-001](../by-category/17-performance.md#prf-001-fast-initial-load): Fast Initial Load
- [PRF-003](../by-category/17-performance.md#prf-003-display-loading-indicators): Display Loading Indicators

### Error Handling
- [ERR-002](../by-category/18-error-handling.md#err-002-retry-failed-operations): Retry Failed Operations
- [ERR-004](../by-category/18-error-handling.md#err-004-graceful-degradation): Graceful Degradation
- [ERR-005](../by-category/18-error-handling.md#err-005-display-status-notifications): Display Status Notifications

## Optional Stories (Nice to Have)

These stories add advanced capabilities:

### Measurement
- [MEA-001](../by-category/06-measurement.md#mea-001-measure-distance): Measure Distance
- [MEA-002](../by-category/06-measurement.md#mea-002-measure-area): Measure Area

### Drawing
- [DRW-004](../by-category/05-drawing-editing.md#drw-004-draw-circle-feature): Draw Circle Feature

### Controls
- [CTL-002](../by-category/09-controls-ui.md#ctl-002-display-scale-bar): Display Scale Bar
- [CTL-003](../by-category/09-controls-ui.md#ctl-003-display-coordinates): Display Coordinates

### Import/Export
- [IMP-003](../by-category/10-import-export.md#imp-003-export-map-as-image): Export Map as Image

### Styling
- [STY-001](../by-category/11-styling.md#sty-001-style-by-attribute-categorical): Style by Attribute
- [STY-003](../by-category/11-styling.md#sty-003-display-feature-labels): Display Feature Labels

### Projections
- [PRJ-001](../by-category/12-projections.md#prj-001-display-coordinates-in-multiple-formats): Display Coordinates in Multiple Formats

### Compliance
- [CMP-002](../by-category/19-compliance.md#cmp-002-privacy-compliance): Privacy Compliance

### Geofencing
- [GEO-001](../by-category/21-geofencing.md#geo-001-create-geofence-zone): Create Geofence Zone
- [GEO-002](../by-category/21-geofencing.md#geo-002-monitor-geofence-entryexit): Monitor Geofence Entry/Exit
- [GEO-003](../by-category/21-geofencing.md#geo-003-trigger-notifications-on-geofence-events): Trigger Notifications on Geofence Events

## Not Typically Needed

These stories may not be relevant for field collection:

- Layer comparison (LAY-004): Complex desktop feature
- Heatmaps (DIS-004): Analysis, not collection
- PDF export (IMP-004): Desktop functionality
- Embed (ITG-002): Internal use only
- Administration (ADM-*): Handled in back-office

## Example Use Cases

### Inspection App
- Navigate to assigned locations
- Complete inspection checklist at each point
- Capture photos of conditions
- Work offline during site visits
- Sync when back online

### Environmental Survey
- Record species observations with GPS accuracy
- Draw habitat boundaries
- Attach photos and audio recordings
- Track surveyor path
- Work in remote areas without connectivity

### Damage Assessment
- Rapid point collection after events
- Category and severity attributes
- Photo documentation
- Real-time sync for coordination
- Filter to show only your assignments

### Utility Maintenance
- Navigate to work order locations
- Update asset condition
- Record maintenance performed
- Snap to existing infrastructure
- View related asset information

## Key Customization Questions

1. What types of features will be collected?
2. What attributes and validation rules are needed?
3. Is photo/media capture required?
4. What level of GPS accuracy is acceptable?
5. What areas have poor or no connectivity?
6. How large is the offline data area needed?
7. How should sync conflicts be resolved?
8. Is tracking of field worker location required?

## Related Starter Kit

See [Field App Starter Kit](../quick-start/starter-kits/field-app-starter.md) for a copy-paste ready story set.
