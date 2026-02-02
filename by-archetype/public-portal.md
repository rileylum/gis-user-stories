# Public Portal Archetype

Read-only maps for public consumption, emphasizing discoverability, performance, and accessibility.

## Archetype Overview

| Attribute | Description |
|-----------|-------------|
| **Primary Users** | Public User, Viewer |
| **Key Goal** | Enable public access to geographic information |
| **Access Model** | Mostly anonymous, read-only |
| **Editing** | None or minimal (user submissions) |
| **Examples** | City data portals, park maps, transit maps, tourism guides |

## Characteristics

- **Read-only or minimal editing**: Users consume information, not create it
- **High accessibility requirements**: Must serve all users including those with disabilities
- **Performance critical**: Fast loading for casual visitors
- **Mobile-first**: Many users on mobile devices
- **SEO considerations**: Shareable, indexable content
- **Low barrier to entry**: No login required for core functionality

## Core Stories (Must Have)

These stories are essential for a public portal:

### Navigation
- [NAV-001](../by-category/01-navigation.md#nav-001-pan-the-map): Pan the Map
- [NAV-002](../by-category/01-navigation.md#nav-002-zoom-with-mouse-wheel): Zoom with Mouse Wheel
- [NAV-003](../by-category/01-navigation.md#nav-003-zoom-with-double-clicktap): Zoom with Double-Click/Tap
- [NAV-004](../by-category/01-navigation.md#nav-004-zoom-with-pinch-gesture): Zoom with Pinch Gesture
- [NAV-006](../by-category/01-navigation.md#nav-006-reset-view): Reset View

### Display
- [DIS-001](../by-category/03-data-display.md#dis-001-display-basemap): Display Basemap
- [DIS-003](../by-category/03-data-display.md#dis-003-display-vector-features): Display Vector Features

### Interaction
- [INT-001](../by-category/04-feature-interaction.md#int-001-click-to-select-feature): Click to Select Feature
- [INT-004](../by-category/04-feature-interaction.md#int-004-display-feature-popup): Display Feature Popup

### Controls
- [CTL-001](../by-category/09-controls-ui.md#ctl-001-display-zoom-buttons): Display Zoom Buttons
- [CTL-002](../by-category/09-controls-ui.md#ctl-002-display-scale-bar): Display Scale Bar
- [CTL-004](../by-category/09-controls-ui.md#ctl-004-display-attribution): Display Attribution

### Accessibility
- [ACC-001](../by-category/13-accessibility.md#acc-001-keyboard-navigation): Keyboard Navigation
- [CMP-001](../by-category/19-compliance.md#cmp-001-wcag-accessibility-compliance): WCAG Compliance

### Performance
- [PRF-001](../by-category/17-performance.md#prf-001-fast-initial-load): Fast Initial Load
- [ERR-001](../by-category/18-error-handling.md#err-001-display-user-friendly-error-messages): User-Friendly Error Messages

## Recommended Stories (Should Have)

These stories significantly enhance the portal experience:

### Layer Management
- [LAY-001](../by-category/02-layer-management.md#lay-001-toggle-layer-visibility): Toggle Layer Visibility
- [LAY-005](../by-category/02-layer-management.md#lay-005-display-minimapoverview): Display Minimap/Overview

### Display Enhancements
- [DIS-002](../by-category/03-data-display.md#dis-002-switch-between-basemaps): Switch Between Basemaps
- [DIS-005](../by-category/03-data-display.md#dis-005-display-clustered-points): Display Clustered Points

### Interaction
- [INT-003](../by-category/04-feature-interaction.md#int-003-hover-to-highlight-feature): Hover to Highlight Feature
- [INT-005](../by-category/04-feature-interaction.md#int-005-filter-features-by-attribute): Filter Features by Attribute

### Search
- [SRC-001](../by-category/08-search-geocoding.md#src-001-search-by-addressplace): Search by Address/Place

### Controls
- [CTL-005](../by-category/09-controls-ui.md#ctl-005-fullscreen-mode): Fullscreen Mode

### Sharing
- [IMP-005](../by-category/10-import-export.md#imp-005-generate-permalinkshare-url): Generate Permalink
- [ITG-001](../by-category/15-integration.md#itg-001-share-map-view): Share Map View

### Accessibility
- [ACC-002](../by-category/13-accessibility.md#acc-002-screen-reader-support): Screen Reader Support
- [ACC-003](../by-category/13-accessibility.md#acc-003-high-contrast-mode): High Contrast Mode

### Performance
- [PRF-003](../by-category/17-performance.md#prf-003-display-loading-indicators): Display Loading Indicators
- [PRF-004](../by-category/17-performance.md#prf-004-cache-data-efficiently): Cache Data Efficiently

## Optional Stories (Nice to Have)

These stories add polish and advanced functionality:

### Navigation
- [NAV-007](../by-category/01-navigation.md#nav-007-kinetic-panning-momentum): Kinetic Panning

### Layer Management
- [LAY-002](../by-category/02-layer-management.md#lay-002-adjust-layer-opacity): Adjust Layer Opacity

### Display
- [DIS-004](../by-category/03-data-display.md#dis-004-display-heatmap): Display Heatmap

### Styling
- [STY-001](../by-category/11-styling.md#sty-001-style-by-attribute-categorical): Style by Attribute
- [STY-003](../by-category/11-styling.md#sty-003-display-feature-labels): Display Feature Labels

### Location
- [LOC-001](../by-category/07-location-services.md#loc-001-show-my-location): Show My Location

### Export
- [IMP-003](../by-category/10-import-export.md#imp-003-export-map-as-image): Export Map as Image

### Integration
- [ITG-002](../by-category/15-integration.md#itg-002-embed-map-in-website): Embed Map in Website

### Compliance
- [CMP-002](../by-category/19-compliance.md#cmp-002-privacy-compliance): Privacy Compliance

## Not Typically Needed

These stories are usually not applicable to public portals:

- Drawing & Editing (DRW-*): Public portals are read-only
- Measurement tools: Unless specifically relevant
- Data Management (DAT-*): No data upload/management
- Administration (ADM-*): Behind-the-scenes configuration

## Example Use Cases

### City Data Portal
- Show city boundaries, parks, facilities
- Filter by neighborhood or service type
- Popup information with links to services
- High accessibility for all citizens

### Tourism Map
- Points of interest with photos
- Basemap switching (streets vs. satellite)
- Share specific locations
- Mobile-first for travelers

### Transit Map
- Real-time vehicle positions
- Route display and filtering
- Stop information popups
- Performance for frequent updates

## Key Customization Questions

1. What layers and data will be displayed?
2. What is the target geographic extent?
3. Are there legal requirements for attribution?
4. What accessibility level is required (AA, AAA)?
5. Will users be on mobile devices?
6. Should the map be embeddable on other sites?
7. What loading time is acceptable?

## Related Starter Kit

See [Public Portal Starter Kit](../quick-start/starter-kits/public-portal-starter.md) for a copy-paste ready story set.
