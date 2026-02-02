# Public Portal Starter Kit

A copy-paste ready set of user stories for public-facing read-only map applications.

## About This Starter Kit

This kit is designed for:
- City/government data portals
- Tourism and visitor maps
- Public information displays
- Informational web maps

**Total Stories: 24**
**Estimated Total Effort: ~8-12 weeks**

---

## Stories to Include

Copy this section directly into your backlog. Customize the bracketed `[...]` sections.

---

### Foundation - Map Display

#### DIS-001: Display Basemap
> As a visitor, I want to see a background map, so that I have geographic context for the information displayed.

**Acceptance Criteria:**
- [ ] Map displays [OpenStreetMap / Satellite / Custom basemap] by default
- [ ] Basemap loads progressively without blocking the interface
- [ ] Attribution is displayed: [Specify attribution text]

**Priority:** Must Have | **Effort:** Small

---

#### DIS-003: Display Vector Features
> As a visitor, I want to see [feature type] displayed on the map, so that I can see [what the data represents].

**Acceptance Criteria:**
- [ ] [Feature type] displays with appropriate symbology
- [ ] Features are visible at zoom levels [X] to [Y]
- [ ] [Customize: Add specific display requirements]

**Priority:** Must Have | **Effort:** Medium

---

### Foundation - Navigation

#### NAV-001: Pan the Map
> As a visitor, I want to drag the map to move the view, so that I can explore different areas.

**Acceptance Criteria:**
- [ ] Click and drag moves the map smoothly
- [ ] Touch and drag works on mobile devices
- [ ] Map is constrained to [geographic extent or "worldwide"]

**Priority:** Must Have | **Effort:** Small

---

#### NAV-002: Zoom with Mouse Wheel
> As a visitor, I want to zoom using my mouse wheel, so that I can quickly adjust the map scale.

**Acceptance Criteria:**
- [ ] Scroll up zooms in, scroll down zooms out
- [ ] Zoom is centered on cursor position
- [ ] Zoom range is [min] to [max] zoom levels

**Priority:** Must Have | **Effort:** Small

---

#### NAV-003: Zoom with Double-Click/Tap
> As a visitor, I want to double-click or double-tap to zoom in, so that I can quickly focus on an area.

**Acceptance Criteria:**
- [ ] Double-click zooms in one level
- [ ] Double-tap works on touch devices
- [ ] Shift+double-click zooms out

**Priority:** Should Have | **Effort:** Small

---

#### NAV-004: Zoom with Pinch Gesture
> As a mobile visitor, I want to pinch to zoom, so that I can navigate naturally on my device.

**Acceptance Criteria:**
- [ ] Pinch-out zooms in, pinch-in zooms out
- [ ] Gesture feels responsive and smooth
- [ ] Works on all supported touch devices

**Priority:** Must Have | **Effort:** Small

---

#### NAV-006: Reset View
> As a visitor, I want to reset the map to its starting view, so that I can return to the default extent.

**Acceptance Criteria:**
- [ ] "Home" or reset button is visible
- [ ] Clicking resets to [default center] at zoom level [X]
- [ ] Animation provides smooth transition

**Priority:** Should Have | **Effort:** Small

---

### Feature Interaction

#### INT-001: Click to Select Feature
> As a visitor, I want to click on a feature to select it, so that I can see its details.

**Acceptance Criteria:**
- [ ] Clicking a feature highlights it
- [ ] Only one feature is selected at a time
- [ ] Clicking elsewhere deselects

**Priority:** Must Have | **Effort:** Small

---

#### INT-003: Hover to Highlight Feature
> As a visitor, I want features to highlight when I hover over them, so that I know they're interactive.

**Acceptance Criteria:**
- [ ] Feature styling changes on hover
- [ ] Cursor changes to pointer
- [ ] [Customize: Hover effect description]

**Priority:** Should Have | **Effort:** Small

---

#### INT-004: Display Feature Popup
> As a visitor, I want to see a popup with information when I select a feature, so that I can learn about it.

**Acceptance Criteria:**
- [ ] Popup appears near the selected feature
- [ ] Popup displays: [list fields to show]
- [ ] Popup has a close button
- [ ] [Customize: Include links, images, etc.?]

**Priority:** Must Have | **Effort:** Medium

---

### Layer Management

#### LAY-001: Toggle Layer Visibility
> As a visitor, I want to turn layers on and off, so that I can focus on what interests me.

**Acceptance Criteria:**
- [ ] Layer panel lists available layers
- [ ] Each layer has a visibility toggle
- [ ] Changes apply immediately
- [ ] [Customize: Which layers are visible by default?]

**Priority:** Should Have | **Effort:** Small

---

### Search

#### SRC-001: Search by Address/Place
> As a visitor, I want to search for an address or place, so that I can navigate to locations I know.

**Acceptance Criteria:**
- [ ] Search box is prominently displayed
- [ ] Autocomplete suggestions appear while typing
- [ ] Selecting a result zooms to that location
- [ ] Search is limited to [geographic scope]

**Priority:** Should Have | **Effort:** Medium

---

### Controls & UI

#### CTL-001: Display Zoom Buttons
> As a visitor, I want visible zoom buttons, so that I have an obvious way to control zoom.

**Acceptance Criteria:**
- [ ] Zoom in (+) and zoom out (-) buttons are visible
- [ ] Buttons are positioned [top-right / specify location]
- [ ] Buttons are touch-friendly (44x44px minimum)

**Priority:** Must Have | **Effort:** Small

---

#### CTL-002: Display Scale Bar
> As a visitor, I want to see a scale bar, so that I understand distances on the map.

**Acceptance Criteria:**
- [ ] Scale bar displays in [metric / imperial / both]
- [ ] Scale updates with zoom level
- [ ] Scale bar is positioned [bottom-left / specify]

**Priority:** Should Have | **Effort:** Small

---

#### CTL-004: Display Attribution
> As a portal operator, I need proper attribution displayed, so that we comply with data licensing.

**Acceptance Criteria:**
- [ ] Attribution text is visible: [specify text]
- [ ] Attribution includes links where required
- [ ] Attribution is collapsible if lengthy

**Priority:** Must Have | **Effort:** Small

---

#### CTL-005: Fullscreen Mode
> As a visitor, I want to view the map in fullscreen, so that I can maximize my viewing area.

**Acceptance Criteria:**
- [ ] Fullscreen button is available
- [ ] Pressing Escape exits fullscreen
- [ ] All controls remain functional

**Priority:** Nice to Have | **Effort:** Small

---

### Sharing

#### IMP-005: Generate Permalink
> As a visitor, I want to get a link to my current view, so that I can share it or bookmark it.

**Acceptance Criteria:**
- [ ] Share button generates a URL
- [ ] URL captures center, zoom, and visible layers
- [ ] URL can be copied to clipboard
- [ ] Opening the URL restores the view

**Priority:** Should Have | **Effort:** Medium

---

#### ITG-001: Share Map View
> As a visitor, I want to share the map on social media, so that others can see what I'm looking at.

**Acceptance Criteria:**
- [ ] Share options include: [email, Twitter, Facebook, etc.]
- [ ] Shared link opens the same view
- [ ] [Customize: Include QR code option?]

**Priority:** Nice to Have | **Effort:** Small

---

### Accessibility

#### ACC-001: Keyboard Navigation
> As a keyboard user, I want to navigate the map without a mouse, so that I can use the application fully.

**Acceptance Criteria:**
- [ ] All controls are keyboard accessible
- [ ] Tab order is logical
- [ ] Focus indicator is visible
- [ ] Arrow keys pan the map

**Priority:** Must Have | **Effort:** Medium

---

#### ACC-002: Screen Reader Support
> As a screen reader user, I want meaningful information announced, so that I can understand the map content.

**Acceptance Criteria:**
- [ ] Map has accessible name and description
- [ ] Interactive elements have ARIA labels
- [ ] Feature information is accessible

**Priority:** Should Have | **Effort:** Large

---

#### ACC-003: High Contrast Mode
> As a user with visual impairments, I want a high-contrast display option, so that I can see the content clearly.

**Acceptance Criteria:**
- [ ] High-contrast mode is available
- [ ] Contrast meets WCAG AA requirements
- [ ] Preference is saved

**Priority:** Should Have | **Effort:** Medium

---

### Performance

#### PRF-001: Fast Initial Load
> As a visitor, I want the map to load quickly, so that I can start using it without delay.

**Acceptance Criteria:**
- [ ] Map is interactive within [X] seconds on broadband
- [ ] Mobile load time is acceptable on 4G
- [ ] Progress indicator shows during load

**Priority:** Must Have | **Effort:** Medium

---

#### PRF-003: Display Loading Indicators
> As a visitor, I want to see loading progress, so that I know data is being fetched.

**Acceptance Criteria:**
- [ ] Loading indicator appears during data fetch
- [ ] Indicator shows tile loading progress
- [ ] Indicator disappears when complete

**Priority:** Should Have | **Effort:** Small

---

### Error Handling

#### ERR-001: Display User-Friendly Error Messages
> As a visitor, I want clear error messages when something fails, so that I understand what happened.

**Acceptance Criteria:**
- [ ] Errors display in plain language
- [ ] Error suggests what to do next
- [ ] Errors can be dismissed

**Priority:** Must Have | **Effort:** Small

---

### Compliance

#### CMP-001: WCAG Accessibility Compliance
> As a portal operator, I need WCAG 2.1 AA compliance, so that we meet accessibility requirements.

**Acceptance Criteria:**
- [ ] Application passes automated WCAG testing
- [ ] Manual audit confirms compliance
- [ ] Accessibility statement is published

**Priority:** Must Have | **Effort:** Large

---

## Customization Checklist

Before using this kit, fill in:

- [ ] Default basemap source
- [ ] Geographic extent/constraints
- [ ] Data layers to display
- [ ] Feature popup content
- [ ] Attribution text
- [ ] Search geographic scope
- [ ] Social sharing platforms
- [ ] Performance targets
- [ ] Branding requirements

## Related Resources

- [Public Portal Archetype](../../by-archetype/public-portal.md) - Full archetype guide
- [MVP Checklist](../mvp-checklist.md) - Minimum requirements
- [Dependency Graph](../../dependencies/dependency-graph.md) - Story dependencies
