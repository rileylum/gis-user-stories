# Drawing & Editing Stories

Creating and modifying geographic features on the map.

---

## DRW-001: Draw Point Feature

| Attribute | Value |
|-----------|-------|
| **Tier** | Foundation |
| **Personas** | Contributor, Field Worker, Analyst |
| **Archetypes** | Field Collection, Collaborative Editor, Asset Management |
| **Dependencies** | DIS-003, INT-001 |
| **Effort** | Small |

**User Story:**
> As a contributor, I want to place a point on the map by clicking, so that I can mark a specific location.

**Acceptance Criteria:**
- [ ] User can activate point drawing mode
- [ ] Clicking on the map places a point at that location
- [ ] Placed point is immediately visible with appropriate styling
- [ ] User can exit drawing mode when finished
- [ ] _[Customize: Point styling and required attributes]_

**Variations:**
- Single point then exit mode vs. continuous point placement
- Point placement with immediate attribute form
- GPS-assisted point placement (use current location)
- Snapping to existing features or grid

**Customization Prompts:**
- What symbol/icon should new points use?
- Should the user be prompted to enter attributes immediately after placement?
- Should point placement use snapping to existing features?

**Non-Functional Considerations:**
- **Performance**: Point placement should be instant
- **Accessibility**: Must support keyboard-based placement (Enter at map center)
- **Mobile**: Touch placement should work with single tap

**Related Stories:** DRW-002, DRW-003, DRW-006, DRW-008

---

## DRW-002: Draw Line Feature

| Attribute | Value |
|-----------|-------|
| **Tier** | Foundation |
| **Personas** | Contributor, Field Worker, Analyst |
| **Archetypes** | Field Collection, Collaborative Editor, Asset Management |
| **Dependencies** | DIS-003, INT-001 |
| **Effort** | Medium |

**User Story:**
> As a contributor, I want to draw a line by clicking a series of points, so that I can represent linear features like roads or paths.

**Acceptance Criteria:**
- [ ] User can activate line drawing mode
- [ ] Each click adds a vertex to the line
- [ ] Line segments display between vertices as they're added
- [ ] Double-click or Enter key completes the line
- [ ] Escape key cancels the current line
- [ ] _[Customize: Minimum vertices and line styling]_

**Variations:**
- Freehand drawing (continuous path while dragging)
- Snapping to existing vertices or features
- Undo last vertex while drawing
- Show distance as drawing progresses

**Customization Prompts:**
- What is the minimum number of vertices for a valid line?
- Should the line show running distance while drawing?
- Should snapping be enabled?

**Non-Functional Considerations:**
- **Performance**: Line drawing should be smooth even for complex paths
- **Accessibility**: Must support keyboard-based vertex placement
- **Mobile**: Touch vertices may need extra confirmation to prevent accidental placement

**Related Stories:** DRW-001, DRW-003, DRW-005, DRW-008, DRW-009

---

## DRW-003: Draw Polygon Feature

| Attribute | Value |
|-----------|-------|
| **Tier** | Foundation |
| **Personas** | Contributor, Field Worker, Analyst |
| **Archetypes** | Field Collection, Collaborative Editor, Asset Management, Analysis Tool |
| **Dependencies** | DIS-003, INT-001 |
| **Effort** | Medium |

**User Story:**
> As a contributor, I want to draw a polygon by clicking vertices, so that I can represent area features like parcels or zones.

**Acceptance Criteria:**
- [ ] User can activate polygon drawing mode
- [ ] Each click adds a vertex to the polygon
- [ ] Polygon preview shows the shape closing back to the first vertex
- [ ] Double-click or Enter key completes the polygon
- [ ] Polygon must have at least 3 vertices to be valid
- [ ] _[Customize: Polygon styling and area display]_

**Variations:**
- Freehand polygon drawing
- Rectangle tool (two corners)
- Show area as drawing progresses
- Hole creation for donuts/complex polygons

**Customization Prompts:**
- Should the polygon show area while drawing?
- Should the tool support creating holes (interior rings)?
- Should snapping be enabled for polygon vertices?

**Non-Functional Considerations:**
- **Performance**: Complex polygons should render smoothly
- **Accessibility**: Must support keyboard-based drawing
- **Mobile**: Consider vertex undo for accidental taps

**Related Stories:** DRW-001, DRW-002, DRW-004, DRW-005, DRW-008, DRW-009

---

## DRW-004: Draw Circle Feature

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Contributor, Analyst |
| **Archetypes** | Analysis Tool, Asset Management |
| **Dependencies** | DRW-003 |
| **Effort** | Small |

**User Story:**
> As a contributor, I want to draw a circle by specifying center and radius, so that I can represent circular areas or buffers.

**Acceptance Criteria:**
- [ ] User can activate circle drawing mode
- [ ] First click sets the center point
- [ ] Dragging or second click sets the radius
- [ ] Circle preview shows current size with radius displayed
- [ ] Circle can be stored as polygon (approximated) or true circle
- [ ] _[Customize: Circle representation and radius units]_

**Variations:**
- Enter radius numerically instead of drawing
- Click center, then drag to set radius
- Ellipse drawing (two radii)
- Geodetic vs. planar circle calculation

**Customization Prompts:**
- Should the circle be stored as a polygon or as center/radius?
- What units should the radius display use?
- Should geodetic calculations be used for accurate circles?

**Non-Functional Considerations:**
- **Performance**: Circle preview should update smoothly while dragging
- **Accessibility**: Must support keyboard-based radius entry
- **Mobile**: Touch-friendly dragging with visual feedback

**Related Stories:** DRW-003, MEA-002

---

## DRW-005: Freehand Drawing

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Contributor, Field Worker |
| **Archetypes** | Field Collection, Collaborative Editor |
| **Dependencies** | DRW-002, DRW-003 |
| **Effort** | Medium |

**User Story:**
> As a contributor, I want to draw by dragging my finger or cursor continuously, so that I can sketch organic shapes quickly.

**Acceptance Criteria:**
- [ ] User can activate freehand drawing mode
- [ ] Dragging creates a continuous line following the cursor/finger
- [ ] Releasing the drag completes the shape
- [ ] Lines can be drawn as open paths
- [ ] Polygons can be closed by returning near the start point
- [ ] _[Customize: Simplification tolerance]_

**Variations:**
- Automatic simplification of drawn path
- Smoothing algorithm for cleaner curves
- Choose between line and polygon mode before drawing
- Pressure sensitivity (if supported by device)

**Customization Prompts:**
- How much should the path be simplified after drawing?
- Should freehand mode create lines, polygons, or either?
- Should there be smoothing applied to the result?

**Non-Functional Considerations:**
- **Performance**: Must capture points quickly for smooth path; simplify on completion
- **Accessibility**: Alternative to freehand must be available
- **Mobile**: Primary use case for touch devices

**Related Stories:** DRW-002, DRW-003

---

## DRW-006: Edit Feature Geometry

| Attribute | Value |
|-----------|-------|
| **Tier** | Foundation |
| **Personas** | Contributor, Field Worker, Administrator |
| **Archetypes** | Field Collection, Collaborative Editor, Asset Management |
| **Dependencies** | INT-001, DRW-001, DRW-002, DRW-003 |
| **Effort** | Medium |

**User Story:**
> As a contributor, I want to edit the shape of an existing feature, so that I can correct or update its geometry.

**Acceptance Criteria:**
- [ ] User can select a feature to enter edit mode
- [ ] Vertices are displayed and can be dragged to new positions
- [ ] Midpoint handles allow adding new vertices
- [ ] Vertices can be deleted (context menu or Delete key)
- [ ] Changes can be saved or cancelled
- [ ] _[Customize: Edit permissions and validation]_

**Variations:**
- Reshape entire feature by dragging edges
- Rotate or scale feature as a whole
- Split feature into multiple parts
- Merge multiple features into one

**Customization Prompts:**
- Which users have permission to edit features?
- Should geometry validation be enforced (e.g., no self-intersection)?
- Should edits be saved immediately or explicitly confirmed?

**Non-Functional Considerations:**
- **Performance**: Edit interactions must be smooth
- **Accessibility**: Keyboard navigation between vertices; Enter to confirm
- **Mobile**: Touch-friendly vertex handles (larger hit targets)

**Related Stories:** DRW-007, DRW-008, DRW-009

---

## DRW-007: Move Feature

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Contributor, Field Worker |
| **Archetypes** | Field Collection, Collaborative Editor, Asset Management |
| **Dependencies** | INT-001, DRW-006 |
| **Effort** | Small |

**User Story:**
> As a contributor, I want to move a feature to a new location, so that I can correct its position.

**Acceptance Criteria:**
- [ ] User can select a feature to move
- [ ] Dragging the feature moves the entire geometry
- [ ] Feature preview shows position while dragging
- [ ] Release confirms the new position
- [ ] Escape cancels the move
- [ ] _[Customize: Move snap settings]_

**Variations:**
- Move by entering coordinate offset
- Move multiple selected features together
- Snap to other features while moving
- Copy and move (duplicate)

**Customization Prompts:**
- Should moving snap to other features or a grid?
- Should users be able to move features by entering coordinates?
- Should move be available for multi-selection?

**Non-Functional Considerations:**
- **Performance**: Feature should follow cursor without lag
- **Accessibility**: Must support keyboard-based movement (arrow keys)
- **Mobile**: Touch-friendly with clear drag handles

**Related Stories:** DRW-006, DRW-008

---

## DRW-008: Delete Feature

| Attribute | Value |
|-----------|-------|
| **Tier** | Foundation |
| **Personas** | Contributor, Field Worker, Administrator |
| **Archetypes** | Field Collection, Collaborative Editor, Asset Management |
| **Dependencies** | INT-001 |
| **Effort** | Small |

**User Story:**
> As a contributor, I want to delete a feature from the map, so that I can remove incorrect or obsolete data.

**Acceptance Criteria:**
- [ ] User can select a feature to delete
- [ ] Delete action is available (button, context menu, or Delete key)
- [ ] Confirmation prompt before deletion (if configured)
- [ ] Feature is removed from the map immediately
- [ ] Deletion can be undone (if undo is available)
- [ ] _[Customize: Confirmation requirement and soft delete]_

**Variations:**
- Soft delete (mark as deleted, don't remove)
- Bulk delete of multiple selected features
- Delete with reason/comment
- Admin-only delete for certain feature types

**Customization Prompts:**
- Should deletion require confirmation?
- Is soft delete (archive) needed instead of permanent delete?
- Who has permission to delete features?

**Non-Functional Considerations:**
- **Performance**: Deletion should be fast
- **Accessibility**: Delete action must be keyboard accessible
- **Mobile**: Confirm dialog should be modal and touch-friendly

**Related Stories:** DRW-006, DRW-007, INT-001

---

## DRW-009: Snap to Features

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Contributor, Analyst |
| **Archetypes** | Collaborative Editor, Asset Management, Analysis Tool |
| **Dependencies** | DRW-002, DRW-003, DRW-006 |
| **Effort** | Medium |

**User Story:**
> As a contributor, I want new vertices to snap to existing features, so that I can create accurate, connected geometries.

**Acceptance Criteria:**
- [ ] When drawing near an existing vertex, cursor snaps to it
- [ ] When drawing near an edge, cursor snaps to the nearest point on that edge
- [ ] Visual indicator shows when snapping is active
- [ ] Snapping can be toggled on/off
- [ ] _[Customize: Snap tolerance and layer priority]_

**Variations:**
- Snap to grid instead of/in addition to features
- Snap to specific layers only
- Different snap modes (vertex, edge, intersection)
- Keyboard modifier to temporarily disable snapping

**Customization Prompts:**
- What is the snapping tolerance distance in pixels?
- Which layers should be snap targets?
- Should grid snapping be available?
- What snap modes are needed (vertex, edge, both)?

**Non-Functional Considerations:**
- **Performance**: Snap detection must be real-time
- **Accessibility**: Announce when snapping occurs
- **Mobile**: May need larger snap tolerance for touch input

**Related Stories:** DRW-002, DRW-003, DRW-006, DRW-007

---

## Summary

| ID | Story | Tier | Effort |
|----|-------|------|--------|
| DRW-001 | Draw Point Feature | Foundation | Small |
| DRW-002 | Draw Line Feature | Foundation | Medium |
| DRW-003 | Draw Polygon Feature | Foundation | Medium |
| DRW-004 | Draw Circle Feature | Standard | Small |
| DRW-005 | Freehand Drawing | Enhanced | Medium |
| DRW-006 | Edit Feature Geometry | Foundation | Medium |
| DRW-007 | Move Feature | Standard | Small |
| DRW-008 | Delete Feature | Foundation | Small |
| DRW-009 | Snap to Features | Enhanced | Medium |
