# Routing & Directions Stories

Route calculation and navigation functionality for turn-by-turn directions and service area analysis.

---

## RTE-001: Calculate Route Between Points

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Public User, Viewer, Field Worker, Analyst |
| **Archetypes** | Field Collection, Public Portal, Analysis Tool |
| **Dependencies** | NAV-001, DIS-003 |
| **Effort** | Medium |

**User Story:**
> As a map user, I want to calculate a route between two or more locations, so that I can see the path and distance for travel planning.

**Acceptance Criteria:**
- [ ] User can specify an origin point (click, search, or current location)
- [ ] User can specify a destination point (click, search, or address)
- [ ] Route is calculated and displayed on the map as a line
- [ ] Route summary shows total distance and estimated travel time
- [ ] Route updates if origin or destination changes
- [ ] _[Customize: Define routing provider/service to use]_

**Variations:**
- Multiple transportation modes (driving, walking, cycling, transit)
- Real-time traffic consideration
- Avoid specific road types or areas
- Alternative routes display

**Customization Prompts:**
- What transportation modes should be supported?
- Should real-time traffic data influence route calculations?
- What routing service will be used (OSRM, GraphHopper, Mapbox, etc.)?
- Should routing work offline with pre-downloaded road networks?

**Non-Functional Considerations:**
- **Performance**: Route calculation should complete within 3 seconds for typical distances
- **Accessibility**: Route summary must be screen reader accessible
- **Mobile**: Touch-friendly waypoint selection

**Related Stories:** RTE-002, RTE-003, RTE-004, SRC-001, LOC-001

---

## RTE-002: Display Turn-by-Turn Directions

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Public User, Viewer, Field Worker |
| **Archetypes** | Field Collection, Public Portal |
| **Dependencies** | RTE-001 |
| **Effort** | Medium |

**User Story:**
> As a map user, I want to see turn-by-turn directions for my route, so that I can follow step-by-step navigation instructions.

**Acceptance Criteria:**
- [ ] Directions panel shows ordered list of navigation steps
- [ ] Each step includes instruction text (e.g., "Turn right onto Main St")
- [ ] Distance and/or time shown for each segment
- [ ] Clicking a step highlights that segment on the map
- [ ] Current step is highlighted during navigation
- [ ] _[Customize: Define instruction detail level]_

**Variations:**
- Voice-read directions for hands-free navigation
- Compact vs. detailed instruction views
- Printable direction sheets
- Maneuver icons (turn arrows, merge symbols)

**Customization Prompts:**
- Should directions include visual maneuver icons?
- Is voice navigation needed for mobile use?
- Should users be able to print directions?
- What language(s) should directions support?

**Non-Functional Considerations:**
- **Performance**: Directions should load as route is calculated
- **Accessibility**: Directions list must be navigable via keyboard and screen reader
- **Mobile**: Directions panel should not obscure map on small screens

**Related Stories:** RTE-001, RTE-003

---

## RTE-003: Add Route Waypoints/Stops

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Public User, Field Worker, Analyst |
| **Archetypes** | Field Collection, Analysis Tool |
| **Dependencies** | RTE-001 |
| **Effort** | Medium |

**User Story:**
> As a map user, I want to add intermediate stops to my route, so that I can plan a multi-stop journey.

**Acceptance Criteria:**
- [ ] User can add waypoints between origin and destination
- [ ] Waypoints can be added by clicking map or entering address
- [ ] Route recalculates to include all waypoints in order
- [ ] User can reorder waypoints by dragging
- [ ] User can remove individual waypoints
- [ ] _[Customize: Define maximum number of waypoints]_

**Variations:**
- Optimize waypoint order for shortest total route
- Named waypoints (e.g., "Lunch stop")
- Time windows for each stop
- Different transportation mode between segments

**Customization Prompts:**
- How many waypoints should be allowed?
- Should route optimization be available to reorder stops?
- Should each waypoint allow notes or scheduled times?
- Should different travel modes be allowed between waypoints?

**Non-Functional Considerations:**
- **Performance**: Route should recalculate quickly when waypoints change
- **Accessibility**: Waypoint list must be keyboard reorderable
- **Mobile**: Drag-to-reorder must work with touch

**Related Stories:** RTE-001, RTE-002, RTE-004

---

## RTE-004: Set Route Preferences

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Public User, Field Worker |
| **Archetypes** | Field Collection, Public Portal |
| **Dependencies** | RTE-001 |
| **Effort** | Small |

**User Story:**
> As a map user, I want to set route preferences like avoiding tolls or highways, so that I can customize my route to my travel needs.

**Acceptance Criteria:**
- [ ] User can select route optimization (fastest, shortest, most economical)
- [ ] User can toggle avoidances (tolls, highways, ferries, unpaved roads)
- [ ] Route recalculates when preferences change
- [ ] Preferences are saved for the session or user profile
- [ ] _[Customize: Define available preference options]_

**Variations:**
- Vehicle-specific preferences (truck height/weight restrictions)
- Accessibility preferences (wheelchair accessible routes)
- Scenic route option
- Carbon footprint optimization

**Customization Prompts:**
- What route optimization options are needed?
- What avoidance options should be available?
- Should preferences persist across sessions?
- Are vehicle-specific constraints needed?

**Non-Functional Considerations:**
- **Performance**: Preference changes should trigger fast recalculation
- **Accessibility**: Preference controls must be keyboard and screen reader accessible
- **Mobile**: Preferences should be in a collapsible panel to save space

**Related Stories:** RTE-001, RTE-003

---

## RTE-005: Calculate Service Areas/Isochrones

| Attribute | Value |
|-----------|-------|
| **Tier** | Specialized |
| **Personas** | Analyst |
| **Archetypes** | Analysis Tool |
| **Dependencies** | RTE-001, DRW-003 |
| **Effort** | Large |

**User Story:**
> As an analyst, I want to generate service area polygons based on travel time or distance, so that I can analyze accessibility and coverage.

**Acceptance Criteria:**
- [ ] User can select a center point for the service area
- [ ] User can specify time intervals (e.g., 5, 10, 15 minutes) or distance bands
- [ ] Isochrone polygons are generated and displayed on the map
- [ ] Multiple intervals shown as concentric polygons with different colors
- [ ] User can export isochrone polygons as GeoJSON
- [ ] _[Customize: Define maximum time/distance and intervals]_

**Variations:**
- Reverse isochrones (areas that can reach a point)
- Multiple origin points for combined service areas
- Different transportation modes
- Contour lines vs. filled polygons

**Customization Prompts:**
- What time/distance intervals are meaningful for your analysis?
- Should multiple transportation modes be supported?
- Is reverse isochrone analysis needed?
- Should isochrones be exportable for further analysis?

**Non-Functional Considerations:**
- **Performance**: Isochrone calculation may take several seconds for complex areas
- **Accessibility**: Results summary must be screen reader accessible
- **Mobile**: Less common on mobile; may be desktop-focused

**Related Stories:** RTE-001, GPR-001, INT-005

---

## Summary

| ID | Story | Tier | Effort |
|----|-------|------|--------|
| RTE-001 | Calculate Route Between Points | Enhanced | Medium |
| RTE-002 | Display Turn-by-Turn Directions | Enhanced | Medium |
| RTE-003 | Add Route Waypoints/Stops | Enhanced | Medium |
| RTE-004 | Set Route Preferences | Enhanced | Small |
| RTE-005 | Calculate Service Areas/Isochrones | Specialized | Large |
