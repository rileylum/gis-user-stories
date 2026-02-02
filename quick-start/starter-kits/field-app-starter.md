# Field App Starter Kit

A copy-paste ready set of user stories for mobile field data collection applications.

## About This Starter Kit

This kit is designed for:
- Field inspection apps
- Survey and data collection
- Environmental monitoring
- Damage assessment
- Maintenance work orders

**Total Stories: 28**
**Estimated Total Effort: ~12-16 weeks**

---

## Stories to Include

Copy this section directly into your backlog. Customize the bracketed `[...]` sections.

---

### Foundation - Map Display

#### DIS-001: Display Basemap
> As a field worker, I want to see a background map, so that I can orient myself in the field.

**Acceptance Criteria:**
- [ ] Map displays [Basemap type] by default
- [ ] [Satellite/aerial] option available for field navigation
- [ ] Basemap loads quickly on mobile networks

**Priority:** Must Have | **Effort:** Small

---

#### DIS-003: Display Vector Features
> As a field worker, I want to see existing [feature type] on the map, so that I know what's already been collected.

**Acceptance Criteria:**
- [ ] [Feature type] displays with distinguishing symbols
- [ ] My collected features are visually distinct
- [ ] Features are visible at appropriate zoom levels

**Priority:** Must Have | **Effort:** Medium

---

### Navigation

#### NAV-001: Pan the Map
> As a field worker, I want to drag the map to move the view, so that I can navigate to my work area.

**Acceptance Criteria:**
- [ ] Touch and drag is smooth and responsive
- [ ] Works well with one hand on a phone
- [ ] [Customize: Map extent constraints if any]

**Priority:** Must Have | **Effort:** Small

---

#### NAV-004: Zoom with Pinch Gesture
> As a field worker, I want to pinch to zoom, so that I can quickly adjust the view on my device.

**Acceptance Criteria:**
- [ ] Pinch zoom is responsive
- [ ] Zoom range is appropriate for field work: [min] to [max]
- [ ] Works with work gloves on (if applicable)

**Priority:** Must Have | **Effort:** Small

---

#### NAV-005: Rotate the Map
> As a field worker, I want to rotate the map to match my orientation, so that navigation is intuitive.

**Acceptance Criteria:**
- [ ] Two-finger rotation works
- [ ] Compass indicator shows current bearing
- [ ] Tap compass to reset to north

**Priority:** Should Have | **Effort:** Medium

---

#### NAV-006: Reset View
> As a field worker, I want to reset to my current location, so that I can quickly reorient.

**Acceptance Criteria:**
- [ ] "My location" button centers on GPS position
- [ ] Works as expected after map manipulation

**Priority:** Should Have | **Effort:** Small

---

### Location Services

#### LOC-001: Show My Location
> As a field worker, I want to see my current location on the map, so that I know where I am.

**Acceptance Criteria:**
- [ ] Blue dot or marker shows my position
- [ ] Accuracy circle shows GPS uncertainty
- [ ] Location updates as I move

**Priority:** Must Have | **Effort:** Small

---

#### LOC-002: Track My Location
> As a field worker, I want continuous location tracking, so that the map follows me as I work.

**Acceptance Criteria:**
- [ ] Toggle for continuous tracking
- [ ] Map optionally follows my location
- [ ] Battery usage is reasonable: [specify target]
- [ ] [Customize: Record track/breadcrumb trail?]

**Priority:** Should Have | **Effort:** Medium

---

#### LOC-003: Center Map on My Location
> As a field worker, I want to quickly center on my location, so that I can see nearby features.

**Acceptance Criteria:**
- [ ] Single tap centers on current GPS position
- [ ] Zooms to appropriate level for field work
- [ ] Works from any current view

**Priority:** Must Have | **Effort:** Small

---

#### LOC-004: Show Location Accuracy
> As a field worker, I want to see GPS accuracy, so that I know if the location is good enough for data collection.

**Acceptance Criteria:**
- [ ] Accuracy shown in meters
- [ ] Color coding: green (<[X]m), yellow (<[Y]m), red (>[Y]m)
- [ ] [Customize: Block collection if accuracy too poor?]

**Priority:** Must Have | **Effort:** Small

---

### Data Collection - Drawing

#### DRW-001: Draw Point Feature
> As a field worker, I want to place a point on the map, so that I can mark a location for data collection.

**Acceptance Criteria:**
- [ ] Tap to place point at that location
- [ ] Option to place at current GPS location
- [ ] Attribute form opens after placement
- [ ] [Customize: Photo capture on creation?]

**Priority:** Must Have | **Effort:** Small

---

#### DRW-002: Draw Line Feature
> As a field worker, I want to draw a line on the map, so that I can trace linear features like [roads, pipes, boundaries].

**Acceptance Criteria:**
- [ ] Tap to add vertices
- [ ] Double-tap or button to complete
- [ ] Undo last vertex option
- [ ] [Customize: Track recording option?]

**Priority:** [If needed] | **Effort:** Medium

---

#### DRW-003: Draw Polygon Feature
> As a field worker, I want to draw a polygon, so that I can mark area features like [damage zones, habitats, parcels].

**Acceptance Criteria:**
- [ ] Tap to add vertices
- [ ] Auto-close to first point
- [ ] Area displayed while drawing
- [ ] Minimum 3 vertices required

**Priority:** [If needed] | **Effort:** Medium

---

#### DRW-005: Freehand Drawing
> As a field worker, I want to draw by dragging my finger, so that I can quickly sketch boundaries.

**Acceptance Criteria:**
- [ ] Drag to draw continuous path
- [ ] Path is simplified on completion
- [ ] Works for both lines and polygons

**Priority:** Nice to Have | **Effort:** Medium

---

#### DRW-006: Edit Feature Geometry
> As a field worker, I want to edit features I've collected, so that I can correct mistakes.

**Acceptance Criteria:**
- [ ] Select feature to enter edit mode
- [ ] Drag vertices to move them
- [ ] Delete vertices if needed
- [ ] Save or cancel edits

**Priority:** Must Have | **Effort:** Medium

---

#### DRW-008: Delete Feature
> As a field worker, I want to delete a feature, so that I can remove incorrect entries.

**Acceptance Criteria:**
- [ ] Delete option for selected feature
- [ ] Confirmation before deletion
- [ ] [Customize: Soft delete or permanent?]

**Priority:** Must Have | **Effort:** Small

---

### Feature Interaction

#### INT-001: Click to Select Feature
> As a field worker, I want to tap a feature to select it, so that I can view or edit it.

**Acceptance Criteria:**
- [ ] Tap selects nearest feature
- [ ] Selected feature is highlighted
- [ ] Tap elsewhere to deselect

**Priority:** Must Have | **Effort:** Small

---

#### INT-004: Display Feature Popup
> As a field worker, I want to see feature attributes, so that I can review collected data.

**Acceptance Criteria:**
- [ ] Popup shows: [list key fields]
- [ ] Edit button opens attribute form
- [ ] Works for my data and reference data

**Priority:** Must Have | **Effort:** Medium

---

### Search

#### SRC-001: Search by Address/Place
> As a field worker, I want to search for an address, so that I can navigate to my next assignment.

**Acceptance Criteria:**
- [ ] Search box accepts addresses
- [ ] Results zoom to location
- [ ] Works with partial addresses

**Priority:** Should Have | **Effort:** Medium

---

### Controls

#### CTL-001: Display Zoom Buttons
> As a field worker, I want zoom buttons, so that I have precise zoom control on a small screen.

**Acceptance Criteria:**
- [ ] Zoom buttons are large enough for field use (50x50px+)
- [ ] Position doesn't interfere with map use
- [ ] Works with work gloves

**Priority:** Must Have | **Effort:** Small

---

#### CTL-006: Display Compass
> As a field worker, I want a compass indicator, so that I know the map orientation.

**Acceptance Criteria:**
- [ ] Compass shows current bearing
- [ ] Tap to reset to north
- [ ] Visible when map is rotated

**Priority:** Should Have | **Effort:** Small

---

### Layer Management

#### LAY-001: Toggle Layer Visibility
> As a field worker, I want to toggle layers, so that I can see relevant reference data.

**Acceptance Criteria:**
- [ ] Simple layer toggle UI
- [ ] [List available layers]
- [ ] State persists during session

**Priority:** Should Have | **Effort:** Small

---

### Offline & Sync

#### PRF-002: Offline Capability
> As a field worker, I want to work offline, so that I can collect data without cell coverage.

**Acceptance Criteria:**
- [ ] Download areas for offline use: [size/scope]
- [ ] View basemap and reference data offline
- [ ] Collected data saved locally
- [ ] Sync when back online

**Priority:** [Critical for field work] | **Effort:** X-Large

---

### Error Handling

#### ERR-001: Display User-Friendly Error Messages
> As a field worker, I want clear error messages, so that I know when something fails in the field.

**Acceptance Criteria:**
- [ ] Errors shown as toasts/banners
- [ ] Clear action recommendations
- [ ] Don't block workflow entirely

**Priority:** Must Have | **Effort:** Small

---

#### ERR-002: Retry Failed Operations
> As a field worker, I want to retry failed saves, so that I don't lose collected data.

**Acceptance Criteria:**
- [ ] Failed saves queued for retry
- [ ] Automatic retry when connection returns
- [ ] Manual retry option available

**Priority:** Must Have | **Effort:** Medium

---

#### ERR-003: Auto-Save Drafts
> As a field worker, I want my work automatically saved, so that I don't lose data if the app crashes.

**Acceptance Criteria:**
- [ ] Unsaved features stored locally
- [ ] Prompt to restore on app restart
- [ ] Clear drafts after successful sync

**Priority:** Must Have | **Effort:** Medium

---

### Authentication

#### ITG-003: Authenticate Users
> As a field worker, I want to log in, so that my collected data is attributed to me.

**Acceptance Criteria:**
- [ ] Login screen on app launch
- [ ] [Specify auth method: username/password, SSO, etc.]
- [ ] Session persists across app restarts
- [ ] Logout option available

**Priority:** Must Have | **Effort:** Large

---

### Performance

#### PRF-003: Display Loading Indicators
> As a field worker, I want to see when data is loading, so that I know the app is working.

**Acceptance Criteria:**
- [ ] Loading indicator during data fetch
- [ ] Sync status indicator
- [ ] Clear feedback on completion

**Priority:** Should Have | **Effort:** Small

---

## Customization Checklist

Before using this kit, fill in:

- [ ] Data types to collect (point, line, polygon)
- [ ] Attribute forms for each feature type
- [ ] Required fields and validation
- [ ] Photo capture requirements
- [ ] Offline area size and coverage
- [ ] GPS accuracy requirements
- [ ] Authentication method
- [ ] Sync behavior and conflict resolution
- [ ] Target devices and OS versions

## Related Resources

- [Field Collection Archetype](../../by-archetype/field-collection.md) - Full archetype guide
- [MVP Checklist](../mvp-checklist.md) - Minimum requirements
- [Dependency Graph](../../dependencies/dependency-graph.md) - Story dependencies
