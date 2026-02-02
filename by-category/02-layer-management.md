# Layer Management Stories

Controlling visibility, order, and appearance of map layers.

---

## LAY-001: Toggle Layer Visibility

| Attribute | Value |
|-----------|-------|
| **Tier** | Foundation |
| **Personas** | Public User, Viewer, Contributor, Analyst, Field Worker |
| **Archetypes** | All |
| **Dependencies** | None |
| **Effort** | Small |

**User Story:**
> As a map user, I want to turn layers on and off, so that I can focus on the information I need.

**Acceptance Criteria:**
- [ ] Layer panel/list displays all available layers
- [ ] Each layer has a visibility toggle (checkbox or eye icon)
- [ ] Layer visibility changes immediately when toggled
- [ ] Layer state is visually indicated (checked/unchecked, visible/hidden icon)
- [ ] _[Customize: Should layer visibility persist between sessions?]_

**Variations:**
- Toggle layer groups (folders) on/off
- "Solo" mode to show only one layer at a time
- Quick toggle all layers on/off

**Customization Prompts:**
- Should users be able to control all layers or only a subset?
- Should layer visibility persist in local storage or user preferences?
- Is there a default layer configuration for first-time users?

**Non-Functional Considerations:**
- **Performance**: Toggling should feel instant (no noticeable delay)
- **Accessibility**: Toggle must be keyboard operable with clear state indication
- **Mobile**: Touch-friendly controls (minimum 44x44px hit targets)

**Related Stories:** LAY-002, LAY-003, CTL-004

---

## LAY-002: Adjust Layer Opacity

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Viewer, Contributor, Analyst |
| **Archetypes** | Analysis Tool, Data Viewer, Asset Management |
| **Dependencies** | LAY-001 |
| **Effort** | Small |

**User Story:**
> As a map user, I want to adjust layer transparency, so that I can see through layers to compare or combine information.

**Acceptance Criteria:**
- [ ] Each layer has an opacity slider (0% to 100%)
- [ ] Opacity changes are applied in real-time as the slider moves
- [ ] Current opacity value is displayed numerically
- [ ] Default opacity is 100% (fully opaque)
- [ ] _[Customize: Should specific layers have different default opacities?]_

**Variations:**
- Preset opacity levels (25%, 50%, 75%, 100%)
- Opacity for layer groups
- Keyboard input for precise opacity values

**Customization Prompts:**
- Which layers should have opacity controls?
- Should opacity be adjustable for basemap layers?
- What is the default opacity for overlay layers?

**Non-Functional Considerations:**
- **Performance**: Real-time opacity changes should be smooth
- **Accessibility**: Slider must be keyboard operable; announce value changes
- **Mobile**: Slider must be easy to manipulate on touch screens

**Related Stories:** LAY-001, LAY-003

---

## LAY-003: Reorder Layers

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Viewer, Contributor, Analyst, Administrator |
| **Archetypes** | Analysis Tool, Data Viewer, Collaborative Editor |
| **Dependencies** | LAY-001 |
| **Effort** | Medium |

**User Story:**
> As a map user, I want to change the drawing order of layers, so that I can control which layers appear on top.

**Acceptance Criteria:**
- [ ] User can drag layers up and down in the layer list
- [ ] Layer at the top of the list is drawn on top of the map
- [ ] Visual feedback during drag (placeholder, ghost, insertion indicator)
- [ ] Layer order updates immediately when dropped
- [ ] _[Customize: Should certain layers be "locked" in position?]_

**Variations:**
- Move to top/bottom buttons instead of drag
- Numbered layer order with input fields
- Separate ordering for basemaps vs. overlays

**Customization Prompts:**
- Should users be able to reorder all layers or only overlays?
- Should basemap layers be in a separate, fixed group?
- Should layer order persist between sessions?

**Non-Functional Considerations:**
- **Performance**: Reordering should not cause visible redraw flicker
- **Accessibility**: Must support keyboard-based reordering (Ctrl+Up/Down)
- **Mobile**: Drag handles must be touch-friendly; consider alternatives

**Related Stories:** LAY-001, LAY-002

---

## LAY-004: Compare Layers with Swipe/Split

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Analyst, Contributor |
| **Archetypes** | Analysis Tool, Data Viewer |
| **Dependencies** | LAY-001, LAY-002 |
| **Effort** | Medium |

**User Story:**
> As an analyst, I want to compare two layers side-by-side or with a swipe tool, so that I can see changes or differences between datasets.

**Acceptance Criteria:**
- [ ] User can select two layers for comparison
- [ ] Swipe mode: draggable divider reveals one layer on each side
- [ ] Swipe position can be adjusted by dragging
- [ ] Current comparison mode is clearly indicated
- [ ] User can exit comparison mode to return to normal view
- [ ] _[Customize: Split mode (side-by-side) in addition to swipe?]_

**Variations:**
- Vertical swipe (left/right reveal)
- Horizontal swipe (top/bottom reveal)
- Split view with synchronized panning
- Flicker mode (rapidly alternate between layers)

**Customization Prompts:**
- Which comparison modes are needed (swipe, split, flicker)?
- Should comparison be limited to specific layer pairs?
- Should the swipe position persist or reset each time?

**Non-Functional Considerations:**
- **Performance**: Rendering both layers simultaneously may impact performance
- **Accessibility**: Keyboard control for swipe position
- **Mobile**: Touch-friendly swipe handle

**Related Stories:** LAY-001, LAY-002, LAY-003

---

## LAY-005: Display Minimap/Overview

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Public User, Viewer, Analyst |
| **Archetypes** | Public Portal, Data Viewer, Analysis Tool |
| **Dependencies** | NAV-001 |
| **Effort** | Small |

**User Story:**
> As a map user, I want to see a minimap showing my current view within the larger area, so that I maintain context while zoomed in.

**Acceptance Criteria:**
- [ ] Small overview map appears in a corner of the main map
- [ ] Overview shows a wider extent than the main map
- [ ] A rectangle or box indicates the current main map extent
- [ ] User can click on the overview to navigate the main map
- [ ] _[Customize: Position and size of overview map]_

**Variations:**
- Collapsible/expandable overview
- Different basemap in overview (simplified)
- Overview shows different layers than main map

**Customization Prompts:**
- Where should the overview map be positioned?
- Should users be able to toggle the overview on/off?
- What basemap should the overview display?
- What size should the overview be?

**Non-Functional Considerations:**
- **Performance**: Overview should not significantly impact main map performance
- **Accessibility**: Overview interactions should be keyboard accessible
- **Mobile**: Consider hiding overview on small screens or making it collapsible

**Related Stories:** NAV-001, NAV-006, CTL-001

---

## Summary

| ID | Story | Tier | Effort |
|----|-------|------|--------|
| LAY-001 | Toggle Layer Visibility | Foundation | Small |
| LAY-002 | Adjust Layer Opacity | Standard | Small |
| LAY-003 | Reorder Layers | Standard | Medium |
| LAY-004 | Compare Layers (Swipe/Split) | Enhanced | Medium |
| LAY-005 | Display Minimap/Overview | Standard | Small |
