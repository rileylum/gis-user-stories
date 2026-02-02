# MVP Checklist

The minimum viable product stories that any web mapping application needs.

## Overview

Before adding advanced features, ensure these foundation stories are in place. This checklist represents the absolute minimum for a functional map application.

## Essential Stories (Required for Any Map)

### Map Display
- [ ] [DIS-001](../by-category/03-data-display.md#dis-001-display-basemap): Display Basemap - *The background map*

### Basic Navigation
- [ ] [NAV-001](../by-category/01-navigation.md#nav-001-pan-the-map): Pan the Map - *Move the view by dragging*
- [ ] [NAV-002](../by-category/01-navigation.md#nav-002-zoom-with-mouse-wheel): Zoom with Mouse Wheel - *Desktop zoom*

### Basic Controls
- [ ] [CTL-001](../by-category/09-controls-ui.md#ctl-001-display-zoom-buttons): Zoom Buttons - *Visual zoom controls*
- [ ] [CTL-004](../by-category/09-controls-ui.md#ctl-004-display-attribution): Attribution - *Legal requirement for most basemaps*

### Basic Error Handling
- [ ] [ERR-001](../by-category/18-error-handling.md#err-001-display-user-friendly-error-messages): Error Messages - *Users need to know when something fails*

**Total: 6 stories**

## Near-Essential Stories (Should Be in v1.0)

Add these for a complete minimum experience:

### Additional Navigation
- [ ] [NAV-003](../by-category/01-navigation.md#nav-003-zoom-with-double-clicktap): Double-Click Zoom - *Common user expectation*
- [ ] [NAV-004](../by-category/01-navigation.md#nav-004-zoom-with-pinch-gesture): Pinch Zoom - *Required for mobile*
- [ ] [NAV-006](../by-category/01-navigation.md#nav-006-reset-view): Reset View - *Return to start*

### Data Display (if showing data)
- [ ] [DIS-003](../by-category/03-data-display.md#dis-003-display-vector-features): Display Features - *Show your data on the map*

### Feature Interaction (if showing data)
- [ ] [INT-001](../by-category/04-feature-interaction.md#int-001-click-to-select-feature): Select Feature - *Click to identify*
- [ ] [INT-004](../by-category/04-feature-interaction.md#int-004-display-feature-popup): Feature Popup - *Show details*

### Basic Accessibility
- [ ] [ACC-001](../by-category/13-accessibility.md#acc-001-keyboard-navigation): Keyboard Navigation - *Foundation for accessibility*

### Performance
- [ ] [PRF-001](../by-category/17-performance.md#prf-001-fast-initial-load): Fast Load - *Users won't wait*
- [ ] [PRF-003](../by-category/17-performance.md#prf-003-display-loading-indicators): Loading Indicators - *Show progress*

**Total: 9 additional stories (15 cumulative)**

## MVP by Archetype

Different application types have different MVP requirements:

### Public Portal MVP
Essential + Near-Essential above, plus:
- [ ] [LAY-001](../by-category/02-layer-management.md#lay-001-toggle-layer-visibility): Layer Toggle - *Users need control*
- [ ] [CMP-001](../by-category/19-compliance.md#cmp-001-wcag-accessibility-compliance): WCAG Compliance - *Public apps must be accessible*

### Data Entry MVP
Essential + Near-Essential above, plus:
- [ ] [DRW-001](../by-category/05-drawing-editing.md#drw-001-draw-point-feature): Draw Points - *Create data*
- [ ] [DRW-008](../by-category/05-drawing-editing.md#drw-008-delete-feature): Delete Features - *Remove mistakes*
- [ ] [ITG-003](../by-category/15-integration.md#itg-003-authenticate-users): Authentication - *Know who's editing*

### Mobile/Field MVP
Essential + Near-Essential above, plus:
- [ ] [LOC-001](../by-category/07-location-services.md#loc-001-show-my-location): My Location - *GPS is expected*
- [ ] [LOC-004](../by-category/07-location-services.md#loc-004-show-location-accuracy): Location Accuracy - *Understand reliability*
- [ ] [ERR-003](../by-category/18-error-handling.md#err-003-auto-save-drafts): Auto-Save - *Don't lose work*

## MVP Validation Questions

Before calling your map "done," verify:

1. **Can users see the map?**
   - Basemap loads and displays
   - Attribution is visible and correct

2. **Can users navigate?**
   - Pan works smoothly
   - Zoom works (wheel, buttons, gestures)
   - Reset to home works

3. **Can users understand the data?**
   - Features display correctly
   - Click to see details works
   - Legends/labels are clear

4. **Is it accessible?**
   - Keyboard navigation works
   - Screen readers can access content
   - Contrast is sufficient

5. **Does it perform?**
   - Loads in acceptable time
   - Responsive during use
   - Errors are communicated

6. **Is it legal?**
   - Attribution displayed
   - Privacy compliant (if collecting data)
   - Accessible (if public-facing)

## Quick Decision Matrix

| Question | If Yes, Add |
|----------|-------------|
| Will it show data layers? | DIS-003, INT-001, INT-004 |
| Will users edit data? | DRW-*, DRW-008, ITG-003 |
| Is it mobile? | NAV-004, LOC-001, LOC-004, ERR-003 |
| Is it public-facing? | ACC-001, ACC-002, CMP-001 |
| Multiple layers? | LAY-001 |
| Need to find places? | SRC-001 |
| Share views? | IMP-005, ITG-001 |

## Next Steps After MVP

Once MVP is validated, typical next additions are:

1. **Better Navigation**: [NAV-007](../by-category/01-navigation.md#nav-007-kinetic-panning-momentum) Kinetic panning
2. **Layer Control**: [LAY-001](../by-category/02-layer-management.md#lay-001-toggle-layer-visibility) Toggle visibility, [LAY-002](../by-category/02-layer-management.md#lay-002-adjust-layer-opacity) Opacity
3. **Search**: [SRC-001](../by-category/08-search-geocoding.md#src-001-search-by-addressplace) Address search
4. **Sharing**: [IMP-005](../by-category/10-import-export.md#imp-005-generate-permalinkshare-url) Permalinks, [ITG-001](../by-category/15-integration.md#itg-001-share-map-view) Share

## Related Resources

- [Dependency Graph](../dependencies/dependency-graph.md) - Understand prerequisites
- [Archetype Guides](../by-archetype/) - Role-specific story sets
- [Starter Kits](starter-kits/) - Copy-paste ready story lists
