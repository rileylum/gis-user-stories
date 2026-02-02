# Measurement Stories

Tools for measuring distances and areas on the map.

---

## MEA-001: Measure Distance

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Public User, Viewer, Analyst, Field Worker |
| **Archetypes** | Public Portal, Analysis Tool, Field Collection, Asset Management |
| **Dependencies** | NAV-001, DIS-001 |
| **Effort** | Medium |

**User Story:**
> As a map user, I want to measure the distance between points on the map, so that I can understand real-world distances.

**Acceptance Criteria:**
- [ ] User can activate distance measurement mode
- [ ] Clicking on the map adds measurement points
- [ ] Line segments are drawn between consecutive points
- [ ] Running total distance is displayed as points are added
- [ ] Double-click or Enter completes the measurement
- [ ] Measurement can be cleared to start over
- [ ] _[Customize: Distance units and precision]_

**Variations:**
- Single segment measurement (point to point)
- Multi-point path measurement
- Geodetic (great circle) vs. planar calculation
- Measure along existing feature geometry

**Customization Prompts:**
- What unit system should be used (metric, imperial, or both)?
- What precision level is needed (decimals)?
- Should geodetic calculations be used for accuracy on curved Earth?
- Should measurements persist or be temporary?

**Non-Functional Considerations:**
- **Performance**: Distance calculation should be real-time as cursor moves
- **Accessibility**: Must support keyboard-based point placement
- **Mobile**: Touch-friendly with clear visual feedback

**Related Stories:** MEA-002, MEA-003

---

## MEA-002: Measure Area

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Analyst, Contributor, Field Worker |
| **Archetypes** | Analysis Tool, Field Collection, Asset Management |
| **Dependencies** | MEA-001 |
| **Effort** | Medium |

**User Story:**
> As an analyst, I want to measure the area of a region on the map, so that I can calculate land size or coverage.

**Acceptance Criteria:**
- [ ] User can activate area measurement mode
- [ ] Clicking on the map adds vertices of a polygon
- [ ] Polygon preview shows the measured area
- [ ] Area value updates in real-time as vertices are added/moved
- [ ] Double-click or Enter completes the measurement
- [ ] Perimeter is also displayed alongside area
- [ ] _[Customize: Area units and precision]_

**Variations:**
- Rectangle area measurement (two corners)
- Circle area measurement (center and radius)
- Measure existing polygon feature
- Geodetic vs. planar area calculation

**Customization Prompts:**
- What area units should be used (sq meters, hectares, acres, sq km)?
- Should geodetic calculations be used for accurate area?
- Should perimeter also be displayed?
- Should the tool support measuring existing features?

**Non-Functional Considerations:**
- **Performance**: Area calculation should update smoothly during drawing
- **Accessibility**: Must support keyboard-based polygon creation
- **Mobile**: Touch-friendly with undo for accidental vertices

**Related Stories:** MEA-001, MEA-003, DRW-003, DRW-004

---

## MEA-003: Live Measurement Display

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Analyst, Contributor, Field Worker |
| **Archetypes** | Field Collection, Analysis Tool, Asset Management |
| **Dependencies** | MEA-001, MEA-002 |
| **Effort** | Small |

**User Story:**
> As a map user, I want to see distance/area update in real-time as I move my cursor, so that I can find exact measurements interactively.

**Acceptance Criteria:**
- [ ] While measuring, moving the cursor updates the projected measurement
- [ ] For distance: shows what the total would be if clicked at current position
- [ ] For area: shows what the area would be if polygon closed at current position
- [ ] Measurement label follows the cursor or appears at a fixed location
- [ ] Updates are smooth and do not lag behind cursor movement
- [ ] _[Customize: Label position and format]_

**Variations:**
- Tooltip following cursor vs. fixed panel display
- Show both segment length and total length
- Include bearing/direction for distance measurement
- Elevation profile for distance (if terrain data available)

**Customization Prompts:**
- Should the measurement label follow the cursor or be in a fixed panel?
- Should individual segment lengths be shown in addition to totals?
- Should bearing/azimuth be displayed for distance measurements?

**Non-Functional Considerations:**
- **Performance**: Calculation and display must keep up with cursor movement
- **Accessibility**: Announce measurement changes for screen readers
- **Mobile**: Ensure label doesn't obscure touch target areas

**Related Stories:** MEA-001, MEA-002, DRW-002, DRW-003

---

## Summary

| ID | Story | Tier | Effort |
|----|-------|------|--------|
| MEA-001 | Measure Distance | Standard | Medium |
| MEA-002 | Measure Area | Standard | Medium |
| MEA-003 | Live Measurement Display | Enhanced | Small |
