# Collaborative Editor Archetype

Multi-user map editing applications for team-based geographic data management.

## Archetype Overview

| Attribute | Description |
|-----------|-------------|
| **Primary Users** | Contributor, Analyst, Administrator |
| **Key Goal** | Enable multiple users to collaboratively create and maintain geographic data |
| **Access Model** | Authenticated, role-based permissions |
| **Editing** | Full CRUD with version control and conflict resolution |
| **Examples** | Collaborative mapping, wiki-style geodata, crowdsourced mapping, team editing |

## Characteristics

- **Multi-user editing**: Multiple people working on the same dataset
- **Version control**: Track changes, history, and rollback
- **Conflict handling**: Manage concurrent edits gracefully
- **Role-based access**: Different permissions for different users
- **Audit trail**: Who changed what and when
- **Quality control**: Review and approval workflows
- **Real-time updates**: See others' changes (optional)
- **Comments/discussion**: Communicate about features

## Core Stories (Must Have)

These stories are essential for collaborative editing:

### Navigation
- [NAV-001](../by-category/01-navigation.md#nav-001-pan-the-map): Pan the Map
- [NAV-002](../by-category/01-navigation.md#nav-002-zoom-with-mouse-wheel): Zoom with Mouse Wheel
- [NAV-006](../by-category/01-navigation.md#nav-006-reset-view): Reset View

### Display
- [DIS-001](../by-category/03-data-display.md#dis-001-display-basemap): Display Basemap
- [DIS-003](../by-category/03-data-display.md#dis-003-display-vector-features): Display Vector Features

### Layer Management
- [LAY-001](../by-category/02-layer-management.md#lay-001-toggle-layer-visibility): Toggle Layer Visibility
- [LAY-003](../by-category/02-layer-management.md#lay-003-reorder-layers): Reorder Layers

### Feature Interaction
- [INT-001](../by-category/04-feature-interaction.md#int-001-click-to-select-feature): Click to Select Feature
- [INT-002](../by-category/04-feature-interaction.md#int-002-box-select-multiple-features): Box Select Multiple Features
- [INT-004](../by-category/04-feature-interaction.md#int-004-display-feature-popup): Display Feature Popup

### Drawing & Editing
- [DRW-001](../by-category/05-drawing-editing.md#drw-001-draw-point-feature): Draw Point Feature
- [DRW-002](../by-category/05-drawing-editing.md#drw-002-draw-line-feature): Draw Line Feature
- [DRW-003](../by-category/05-drawing-editing.md#drw-003-draw-polygon-feature): Draw Polygon Feature
- [DRW-006](../by-category/05-drawing-editing.md#drw-006-edit-feature-geometry): Edit Feature Geometry
- [DRW-007](../by-category/05-drawing-editing.md#drw-007-move-feature): Move Feature
- [DRW-008](../by-category/05-drawing-editing.md#drw-008-delete-feature): Delete Feature
- [DRW-009](../by-category/05-drawing-editing.md#drw-009-snap-to-features): Snap to Features

### Controls
- [CTL-001](../by-category/09-controls-ui.md#ctl-001-display-zoom-buttons): Display Zoom Buttons
- [CTL-004](../by-category/09-controls-ui.md#ctl-004-display-attribution): Display Attribution

### Integration
- [ITG-003](../by-category/15-integration.md#itg-003-authenticate-users): Authenticate Users

### Administration
- [ADM-002](../by-category/16-administration.md#adm-002-manage-user-permissions): Manage User Permissions

### Error Handling
- [ERR-001](../by-category/18-error-handling.md#err-001-display-user-friendly-error-messages): User-Friendly Error Messages
- [ERR-002](../by-category/18-error-handling.md#err-002-retry-failed-operations): Retry Failed Operations

## Recommended Stories (Should Have)

These stories significantly improve collaboration:

### Navigation
- [NAV-003](../by-category/01-navigation.md#nav-003-zoom-with-double-clicktap): Zoom with Double-Click

### Display
- [DIS-002](../by-category/03-data-display.md#dis-002-switch-between-basemaps): Switch Between Basemaps

### Layer Management
- [LAY-002](../by-category/02-layer-management.md#lay-002-adjust-layer-opacity): Adjust Layer Opacity

### Feature Interaction
- [INT-003](../by-category/04-feature-interaction.md#int-003-hover-to-highlight-feature): Hover to Highlight Feature
- [INT-005](../by-category/04-feature-interaction.md#int-005-filter-features-by-attribute): Filter Features by Attribute

### Drawing & Editing
- [DRW-004](../by-category/05-drawing-editing.md#drw-004-draw-circle-feature): Draw Circle Feature
- [DRW-005](../by-category/05-drawing-editing.md#drw-005-freehand-drawing): Freehand Drawing

### Measurement
- [MEA-001](../by-category/06-measurement.md#mea-001-measure-distance): Measure Distance
- [MEA-002](../by-category/06-measurement.md#mea-002-measure-area): Measure Area

### Search
- [SRC-001](../by-category/08-search-geocoding.md#src-001-search-by-addressplace): Search by Address/Place
- [SRC-002](../by-category/08-search-geocoding.md#src-002-search-by-coordinates): Search by Coordinates

### Controls
- [CTL-003](../by-category/09-controls-ui.md#ctl-003-display-coordinates): Display Coordinates

### Styling
- [STY-001](../by-category/11-styling.md#sty-001-style-by-attribute-categorical): Style by Attribute
- [STY-002](../by-category/11-styling.md#sty-002-display-custom-iconssymbols): Display Custom Icons
- [STY-003](../by-category/11-styling.md#sty-003-display-feature-labels): Display Feature Labels

### Data Management
- [DAT-002](../by-category/14-data-management.md#dat-002-indicate-data-freshness): Indicate Data Freshness
- [DAT-004](../by-category/14-data-management.md#dat-004-data-versioning): Data Versioning

### Administration
- [ADM-001](../by-category/16-administration.md#adm-001-configure-layer-settings): Configure Layer Settings
- [ADM-004](../by-category/16-administration.md#adm-004-set-default-map-configuration): Set Default Map Configuration

### Performance
- [PRF-001](../by-category/17-performance.md#prf-001-fast-initial-load): Fast Initial Load
- [PRF-003](../by-category/17-performance.md#prf-003-display-loading-indicators): Display Loading Indicators

### Error Handling
- [ERR-003](../by-category/18-error-handling.md#err-003-auto-save-drafts): Auto-Save Drafts
- [ERR-004](../by-category/18-error-handling.md#err-004-graceful-degradation): Graceful Degradation

## Optional Stories (Nice to Have)

These stories add advanced collaboration features:

### Navigation
- [NAV-004](../by-category/01-navigation.md#nav-004-zoom-with-pinch-gesture): Zoom with Pinch Gesture

### Measurement
- [MEA-003](../by-category/06-measurement.md#mea-003-live-measurement-display): Live Measurement Display

### Import/Export
- [IMP-001](../by-category/10-import-export.md#imp-001-import-data-file): Import Data File
- [IMP-002](../by-category/10-import-export.md#imp-002-drag-and-drop-import): Drag and Drop Import
- [IMP-003](../by-category/10-import-export.md#imp-003-export-map-as-image): Export Map as Image
- [IMP-005](../by-category/10-import-export.md#imp-005-generate-permalinkshare-url): Generate Permalink

### Data Management
- [DAT-001](../by-category/14-data-management.md#dat-001-upload-data): Upload Data
- [DAT-003](../by-category/14-data-management.md#dat-003-download-data): Download Data

### Projections
- [PRJ-001](../by-category/12-projections.md#prj-001-display-coordinates-in-multiple-formats): Display Coordinates in Multiple Formats
- [PRJ-002](../by-category/12-projections.md#prj-002-transform-coordinates-between-systems): Transform Coordinates

### Integration
- [ITG-001](../by-category/15-integration.md#itg-001-share-map-view): Share Map View
- [ITG-004](../by-category/15-integration.md#itg-004-access-via-api): Access via API

### Compliance
- [CMP-003](../by-category/19-compliance.md#cmp-003-data-governance): Data Governance

### Accessibility
- [ACC-001](../by-category/13-accessibility.md#acc-001-keyboard-navigation): Keyboard Navigation

## Advanced Collaborative Features

Consider these beyond standard stories:

- **Real-time presence**: See who else is viewing/editing
- **Live cursors**: See where other users are working
- **Feature locking**: Prevent concurrent edits to same feature
- **Comments**: Discuss features and changes
- **Notifications**: Alert when features of interest change
- **Review workflow**: Approve changes before publishing
- **Branching**: Work on separate versions, then merge
- **Conflict resolution**: Handle simultaneous edits

## Not Typically Needed

These stories may not be relevant for collaborative editors:

- Offline capability: Editing requires connectivity for collaboration
- Location services: Not field-based (see Field Collection for that)
- Heatmaps/analysis: Focus is on editing, not analysis

## Example Use Cases

### Community Mapping
- Multiple contributors add local knowledge
- Review process for new additions
- Version history for edits
- Discussion on disputed features

### Data Maintenance Team
- Distributed team maintains shared dataset
- Work assignment by region or type
- Quality control workflows
- Change tracking for compliance

### Crowdsourced Mapping
- Public contributions with moderation
- Reputation/trust levels
- Rollback for vandalism
- Attribution of contributors

### Enterprise Geodata
- Central data repository
- Multiple departments editing different layers
- Approval workflows
- Audit trail for compliance

## Key Customization Questions

1. How many concurrent users are expected?
2. What is the conflict resolution strategy?
3. Is real-time collaboration needed, or is save-and-refresh acceptable?
4. What approval workflows are required?
5. What level of audit trail is needed?
6. Should there be feature-level or layer-level locking?
7. Are comments and discussions needed?
8. What are the role definitions and permissions?

## Related Resources

Collaborative editing combines aspects of multiple archetypes. See:
- [Asset Management Archetype](asset-management.md) for similar editing patterns
- [Field Collection Archetype](field-collection.md) if field editing is needed
- [Dependency Graph](../dependencies/dependency-graph.md) for story relationships
