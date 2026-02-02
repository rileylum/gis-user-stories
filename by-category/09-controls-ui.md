# Controls & UI Stories

Map controls and user interface elements.

---

## CTL-001: Display Zoom Buttons

| Attribute | Value |
|-----------|-------|
| **Tier** | Foundation |
| **Personas** | Public User, Viewer, Contributor, Analyst, Field Worker |
| **Archetypes** | All |
| **Dependencies** | NAV-002 |
| **Effort** | Small |

**User Story:**
> As a map user, I want visible zoom in/out buttons, so that I can control the map zoom level without using gestures.

**Acceptance Criteria:**
- [ ] Zoom in (+) and zoom out (-) buttons are visible on the map
- [ ] Clicking zoom in increases the zoom level by one
- [ ] Clicking zoom out decreases the zoom level by one
- [ ] Buttons are disabled at min/max zoom levels
- [ ] Buttons have appropriate hover and active states
- [ ] _[Customize: Button position and styling]_

**Variations:**
- Zoom slider instead of/in addition to buttons
- Zoom to specific level selector
- Animated vs. instant zoom transitions
- Custom button icons

**Customization Prompts:**
- Where should zoom controls be positioned?
- Should a zoom slider be included?
- Should there be a zoom level indicator?
- What are the min/max zoom constraints?

**Non-Functional Considerations:**
- **Performance**: Zoom transitions should be smooth
- **Accessibility**: Buttons must be keyboard accessible; appropriate ARIA labels
- **Mobile**: Buttons must be touch-friendly (minimum 44x44px)

**Related Stories:** NAV-002, NAV-003, NAV-004, NAV-006

---

## CTL-002: Display Scale Bar

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Public User, Viewer, Analyst, Field Worker |
| **Archetypes** | All |
| **Dependencies** | NAV-002 |
| **Effort** | Small |

**User Story:**
> As a map user, I want to see a scale bar, so that I can understand the real-world distances on the map.

**Acceptance Criteria:**
- [ ] Scale bar is displayed in a corner of the map
- [ ] Scale bar updates as zoom level changes
- [ ] Scale shows distance in appropriate units (m, km, ft, mi)
- [ ] Scale bar length adjusts to show round numbers
- [ ] _[Customize: Units and position]_

**Variations:**
- Dual scale (metric and imperial)
- Numeric scale ratio (1:10,000)
- Custom styling/colors
- Hide at certain zoom levels

**Customization Prompts:**
- What unit system should the scale bar use?
- Should dual units (metric and imperial) be shown?
- Where should the scale bar be positioned?
- Should a numeric ratio also be displayed?

**Non-Functional Considerations:**
- **Performance**: Scale updates should be instant with zoom
- **Accessibility**: Scale bar should have alt text for screen readers
- **Mobile**: Should not obstruct other controls

**Related Stories:** CTL-001, CTL-003

---

## CTL-003: Display Coordinates

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Analyst, Field Worker, Contributor |
| **Archetypes** | Analysis Tool, Field Collection, Asset Management |
| **Dependencies** | NAV-001 |
| **Effort** | Small |

**User Story:**
> As an analyst, I want to see the coordinates of my cursor position, so that I can identify precise locations.

**Acceptance Criteria:**
- [ ] Coordinate display shows the current cursor/pointer position
- [ ] Coordinates update in real-time as the cursor moves
- [ ] Coordinates are displayed in a consistent format
- [ ] User can copy coordinates to clipboard
- [ ] _[Customize: Coordinate format and display location]_

**Variations:**
- Toggle between different coordinate formats (DD, DMS, UTM)
- Show map center coordinates instead of cursor
- Click to copy coordinates
- Show elevation if terrain data available

**Customization Prompts:**
- What coordinate format should be used by default?
- Should users be able to switch between formats?
- Where should coordinates be displayed?
- Is click-to-copy needed?

**Non-Functional Considerations:**
- **Performance**: Coordinate updates must not cause lag
- **Accessibility**: Coordinates should be readable by screen readers
- **Mobile**: May need different trigger (tap and hold) since no hover

**Related Stories:** CTL-002, PRJ-001, SRC-002

---

## CTL-004: Display Attribution

| Attribute | Value |
|-----------|-------|
| **Tier** | Foundation |
| **Personas** | Public User, Viewer, Contributor, Analyst, Field Worker |
| **Archetypes** | All |
| **Dependencies** | DIS-001 |
| **Effort** | Small |

**User Story:**
> As an administrator, I need to display proper attribution for map data sources, so that I comply with licensing requirements.

**Acceptance Criteria:**
- [ ] Attribution text is visible on the map
- [ ] Attribution updates when layer sources change
- [ ] Attribution links are clickable
- [ ] Attribution can be collapsed/expanded if lengthy
- [ ] _[Customize: Attribution text and styling]_

**Variations:**
- Collapsible attribution panel
- Attribution in popup/modal instead of on-map
- Logo-based attribution for branded sources
- Custom attribution text

**Customization Prompts:**
- What data sources require attribution?
- Should attribution be collapsible?
- Are there specific branding requirements for data providers?

**Non-Functional Considerations:**
- **Performance**: Minimal impact
- **Accessibility**: Attribution links must be keyboard navigable
- **Mobile**: Collapsible to save screen space

**Related Stories:** DIS-001, DIS-002

---

## CTL-005: Fullscreen Mode

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Public User, Viewer, Analyst |
| **Archetypes** | Public Portal, Data Viewer, Analysis Tool |
| **Dependencies** | None |
| **Effort** | Small |

**User Story:**
> As a map user, I want to view the map in fullscreen mode, so that I can maximize my viewing area.

**Acceptance Criteria:**
- [ ] Fullscreen button is visible on the map
- [ ] Clicking the button enters fullscreen mode
- [ ] Map fills the entire screen in fullscreen mode
- [ ] Exit fullscreen button or Escape key returns to normal view
- [ ] All controls remain functional in fullscreen
- [ ] _[Customize: Fullscreen behavior and button position]_

**Variations:**
- Toggle between fullscreen and embedded view
- Hide certain UI elements in fullscreen
- Persist fullscreen preference
- Keyboard shortcut (F11 fallback)

**Customization Prompts:**
- Should fullscreen mode be available?
- What controls should be visible in fullscreen mode?
- Should any UI elements be hidden in fullscreen?

**Non-Functional Considerations:**
- **Performance**: Transition should be smooth
- **Accessibility**: Escape key must exit fullscreen; screen readers should announce mode
- **Mobile**: Full browser viewport; may behave differently on various devices

**Related Stories:** CTL-001, CTL-002

---

## CTL-006: Display Compass/North Arrow

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Viewer, Analyst, Field Worker |
| **Archetypes** | Field Collection, Analysis Tool, Public Portal |
| **Dependencies** | NAV-005 |
| **Effort** | Small |

**User Story:**
> As a map user, I want to see a compass showing north, so that I know the map's orientation.

**Acceptance Criteria:**
- [ ] Compass/north arrow is displayed on the map
- [ ] Compass rotates when map is rotated
- [ ] Clicking the compass resets rotation to north-up
- [ ] Compass is hidden when map is north-up (optional)
- [ ] _[Customize: Compass styling and visibility]_

**Variations:**
- Always visible vs. only when rotated
- Simple north arrow vs. full compass rose
- Show bearing in degrees
- Custom compass icon

**Customization Prompts:**
- Should the compass always be visible or only when rotated?
- What compass style is preferred (simple arrow, compass rose)?
- Should the current bearing be displayed numerically?

**Non-Functional Considerations:**
- **Performance**: Rotation updates should be smooth
- **Accessibility**: Announce current orientation; click to reset
- **Mobile**: Touch-friendly reset action

**Related Stories:** NAV-005, NAV-006

---

## CTL-007: Display Legend

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Public User, Viewer, Analyst |
| **Archetypes** | Public Portal, Data Viewer, Analysis Tool, Asset Management |
| **Dependencies** | DIS-003, LAY-001 |
| **Effort** | Medium |

**User Story:**
> As a map user, I want to see a legend explaining what the symbols mean, so that I can understand the data displayed on the map.

**Acceptance Criteria:**
- [ ] Legend displays symbols/colors for each visible layer
- [ ] Legend updates when layer visibility changes
- [ ] Legend shows the meaning of graduated/classified symbology
- [ ] Legend can be expanded/collapsed to save space
- [ ] Legend labels are clear and readable
- [ ] _[Customize: Legend position, style, and content]_

**Variations:**
- Integrated with layer panel vs. standalone control
- Interactive legend (click symbol to filter map)
- Collapsible sections per layer
- Dynamic legend based on current map extent (only show features present)
- Print-friendly legend format

**Customization Prompts:**
- Should the legend be always visible or collapsible?
- Should clicking a legend item filter the map?
- Where should the legend be positioned?
- Should the legend show counts of features per category?
- Should the legend include layer descriptions?

**Non-Functional Considerations:**
- **Performance**: Legend should update quickly when layers change
- **Accessibility**: Legend must be readable by screen readers; sufficient color contrast
- **Mobile**: Legend should be collapsible on small screens; consider bottom sheet

**Related Stories:** DIS-003, LAY-001, STY-001, STY-002

---

## Summary

| ID | Story | Tier | Effort |
|----|-------|------|--------|
| CTL-001 | Display Zoom Buttons | Foundation | Small |
| CTL-002 | Display Scale Bar | Standard | Small |
| CTL-003 | Display Coordinates | Standard | Small |
| CTL-004 | Display Attribution | Foundation | Small |
| CTL-005 | Fullscreen Mode | Standard | Small |
| CTL-006 | Display Compass | Standard | Small |
| CTL-007 | Display Legend | Standard | Medium |
