# Search & Geocoding Stories

Finding locations by address, place name, or coordinates.

---

## SRC-001: Search by Address/Place

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Public User, Viewer, Field Worker |
| **Archetypes** | Public Portal, Field Collection, Asset Management |
| **Dependencies** | NAV-001 |
| **Effort** | Medium |

**User Story:**
> As a map user, I want to search for a place or address and go to that location, so that I can quickly navigate to points of interest.

**Acceptance Criteria:**
- [ ] Search box is prominently displayed in the UI
- [ ] User can type an address, place name, or landmark
- [ ] Autocomplete suggestions appear as user types
- [ ] Selecting a result zooms and centers the map on that location
- [ ] Result location is marked on the map
- [ ] _[Customize: Geocoding provider and search scope]_

**Variations:**
- Search within current map extent only
- Search filtered by category (restaurants, parks, etc.)
- Recent searches/favorites
- Search multiple geocoding providers

**Customization Prompts:**
- Which geocoding service should be used?
- Should search be limited to a specific region or country?
- How many autocomplete suggestions should be shown?
- Should search results persist as markers?

**Non-Functional Considerations:**
- **Performance**: Autocomplete should respond within 200ms
- **Accessibility**: Search input must be keyboard navigable; announce results
- **Mobile**: Virtual keyboard should not obscure results

**Related Stories:** SRC-002, SRC-003, NAV-001

---

## SRC-002: Search by Coordinates

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Analyst, Field Worker |
| **Archetypes** | Analysis Tool, Field Collection |
| **Dependencies** | NAV-001 |
| **Effort** | Small |

**User Story:**
> As an analyst, I want to navigate to a specific coordinate location, so that I can find exact positions.

**Acceptance Criteria:**
- [ ] User can enter coordinates in the search box or a dedicated field
- [ ] Multiple coordinate formats are supported (decimal degrees, DMS)
- [ ] Entering valid coordinates centers the map on that location
- [ ] A marker is placed at the coordinate location
- [ ] Invalid coordinate format shows a helpful error message
- [ ] _[Customize: Supported coordinate formats]_

**Variations:**
- Separate latitude and longitude input fields
- Coordinate format dropdown selector
- Paste coordinates from clipboard
- Support for different coordinate reference systems

**Customization Prompts:**
- What coordinate formats should be supported?
- Should coordinates in different CRS be accepted and transformed?
- What precision should be displayed for found locations?

**Non-Functional Considerations:**
- **Performance**: Coordinate parsing should be instant
- **Accessibility**: Input fields must be properly labeled
- **Mobile**: Numeric keyboard for coordinate entry

**Related Stories:** SRC-001, SRC-003, PRJ-001

---

## SRC-003: Reverse Geocode (Click to Address)

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Public User, Field Worker, Analyst |
| **Archetypes** | Public Portal, Field Collection, Analysis Tool |
| **Dependencies** | SRC-001 |
| **Effort** | Small |

**User Story:**
> As a map user, I want to click on the map and see the address of that location, so that I can identify places without knowing their address.

**Acceptance Criteria:**
- [ ] User can activate a "What's here?" or reverse geocode tool
- [ ] Clicking on the map retrieves the address for that point
- [ ] Address is displayed in a popup or panel
- [ ] Coordinates of the clicked point are also shown
- [ ] User can copy the address or coordinates
- [ ] _[Customize: Reverse geocoding provider and detail level]_

**Variations:**
- Right-click context menu option
- Long-press on touch devices
- Show multiple address candidates
- Include what3words or other location codes

**Customization Prompts:**
- How should reverse geocode be triggered (tool, right-click, long-press)?
- What level of address detail is needed (street, city, country)?
- Should what3words or similar systems be included?

**Non-Functional Considerations:**
- **Performance**: Reverse geocode should return within 1 second
- **Accessibility**: Results must be announced to screen readers
- **Mobile**: Long-press is the standard touch gesture

**Related Stories:** SRC-001, SRC-002, INT-004

---

## Summary

| ID | Story | Tier | Effort |
|----|-------|------|--------|
| SRC-001 | Search by Address/Place | Standard | Medium |
| SRC-002 | Search by Coordinates | Standard | Small |
| SRC-003 | Reverse Geocode | Enhanced | Small |
