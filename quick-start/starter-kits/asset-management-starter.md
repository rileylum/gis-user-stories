# Asset Management Starter Kit

A copy-paste ready set of user stories for asset tracking and management applications.

## About This Starter Kit

This kit is designed for:
- Utility infrastructure management
- Fleet and vehicle tracking
- Equipment inventory
- Facility management
- Property/real estate management

**Total Stories: 32**
**Estimated Total Effort: ~14-18 weeks**

---

## Stories to Include

Copy this section directly into your backlog. Customize the bracketed `[...]` sections.

---

### Foundation - Map Display

#### DIS-001: Display Basemap
> As an asset manager, I want to see a background map, so that I can locate assets in geographic context.

**Acceptance Criteria:**
- [ ] Default basemap is [street/satellite/hybrid]
- [ ] Basemap provides sufficient detail for asset location
- [ ] Attribution is properly displayed

**Priority:** Must Have | **Effort:** Small

---

#### DIS-002: Switch Between Basemaps
> As an asset manager, I want to switch basemaps, so that I can see aerial imagery or street context as needed.

**Acceptance Criteria:**
- [ ] At least two basemap options: [street, satellite]
- [ ] Current basemap is indicated
- [ ] Switch preserves current view

**Priority:** Should Have | **Effort:** Small

---

#### DIS-003: Display Asset Features
> As an asset manager, I want to see [asset type] displayed on the map, so that I can see the spatial distribution of our assets.

**Acceptance Criteria:**
- [ ] [Asset type 1] displays with [symbol/icon]
- [ ] [Asset type 2] displays with [symbol/icon]
- [ ] Assets are distinguishable by type and status
- [ ] [Customize: Add all asset types]

**Priority:** Must Have | **Effort:** Medium

---

#### DIS-005: Display Clustered Assets
> As an asset manager, I want nearby assets clustered at low zoom, so that the map remains readable with many assets.

**Acceptance Criteria:**
- [ ] Assets cluster when many are visible
- [ ] Cluster shows count of grouped assets
- [ ] Click cluster to zoom and expand
- [ ] Clusters work for [asset types]

**Priority:** Should Have | **Effort:** Medium

---

### Navigation

#### NAV-001: Pan the Map
> As an asset manager, I want to drag the map, so that I can navigate to different areas.

**Acceptance Criteria:**
- [ ] Click and drag moves smoothly
- [ ] Map extent is [constrained to service area / worldwide]

**Priority:** Must Have | **Effort:** Small

---

#### NAV-002: Zoom with Mouse Wheel
> As an asset manager, I want to zoom with the mouse wheel, so that I can quickly change scale.

**Acceptance Criteria:**
- [ ] Wheel zoom is smooth and centered on cursor
- [ ] Zoom levels range from [overview] to [detail level]

**Priority:** Must Have | **Effort:** Small

---

#### NAV-006: Reset View
> As an asset manager, I want to reset to the default view, so that I can return to the main service area.

**Acceptance Criteria:**
- [ ] Reset button returns to [default center and zoom]
- [ ] Visible and easy to access

**Priority:** Should Have | **Effort:** Small

---

### Layer Management

#### LAY-001: Toggle Asset Layer Visibility
> As an asset manager, I want to toggle asset layers on and off, so that I can focus on specific asset types.

**Acceptance Criteria:**
- [ ] Layer panel lists: [asset type 1, type 2, type 3, ...]
- [ ] Each layer can be toggled independently
- [ ] Layer state persists during session

**Priority:** Must Have | **Effort:** Small

---

#### LAY-002: Adjust Layer Opacity
> As an asset manager, I want to adjust layer opacity, so that I can see overlapping data.

**Acceptance Criteria:**
- [ ] Opacity slider for each layer
- [ ] Changes apply in real-time
- [ ] Useful range from 0% to 100%

**Priority:** Should Have | **Effort:** Small

---

#### LAY-003: Reorder Layers
> As an asset manager, I want to change layer order, so that important layers are on top.

**Acceptance Criteria:**
- [ ] Drag layers to reorder
- [ ] Order reflects drawing order
- [ ] Order persists during session

**Priority:** Nice to Have | **Effort:** Medium

---

### Feature Interaction

#### INT-001: Select Asset
> As an asset manager, I want to click an asset to select it, so that I can view or edit its details.

**Acceptance Criteria:**
- [ ] Click selects the asset
- [ ] Selected asset is highlighted
- [ ] Click elsewhere deselects

**Priority:** Must Have | **Effort:** Small

---

#### INT-002: Box Select Multiple Assets
> As an asset manager, I want to draw a box to select multiple assets, so that I can perform bulk operations.

**Acceptance Criteria:**
- [ ] Shift+drag creates selection box
- [ ] All assets in box are selected
- [ ] Selection count is displayed
- [ ] [Customize: What bulk operations are available?]

**Priority:** Should Have | **Effort:** Medium

---

#### INT-003: Hover to Highlight Asset
> As an asset manager, I want assets to highlight on hover, so that I know what I'm about to select.

**Acceptance Criteria:**
- [ ] Asset styling changes on hover
- [ ] Cursor indicates clickable
- [ ] [Customize: Show tooltip with asset ID?]

**Priority:** Should Have | **Effort:** Small

---

#### INT-004: Display Asset Details
> As an asset manager, I want to see asset details when I select one, so that I can review its information.

**Acceptance Criteria:**
- [ ] Details panel shows: [list key fields]
- [ ] Links to related records: [work orders, history, etc.]
- [ ] Edit button for authorized users
- [ ] [Customize: Include photos, documents?]

**Priority:** Must Have | **Effort:** Medium

---

#### INT-005: Filter Assets by Attribute
> As an asset manager, I want to filter assets by [status, type, date, etc.], so that I can find specific assets.

**Acceptance Criteria:**
- [ ] Filter by: [status, type, age, condition, ...]
- [ ] Multiple filters can be combined
- [ ] Active filters clearly shown
- [ ] Clear all filters option

**Priority:** Must Have | **Effort:** Medium

---

### Asset Editing

#### DRW-001: Add Point Asset
> As an asset manager, I want to place a new asset on the map, so that I can add to our inventory.

**Acceptance Criteria:**
- [ ] Click to place asset location
- [ ] Attribute form opens
- [ ] Required fields: [list required fields]
- [ ] [Customize: GPS option for field placement?]

**Priority:** Must Have | **Effort:** Small

---

#### DRW-002: Add Linear Asset
> As an asset manager, I want to draw a line for [pipes, cables, roads, etc.], so that I can add linear assets.

**Acceptance Criteria:**
- [ ] Click to add vertices
- [ ] Double-click to complete
- [ ] Length displayed while drawing
- [ ] [Customize: Snapping to other features?]

**Priority:** [If linear assets] | **Effort:** Medium

---

#### DRW-003: Add Area Asset
> As an asset manager, I want to draw a polygon for [parcels, zones, buildings, etc.], so that I can add area assets.

**Acceptance Criteria:**
- [ ] Click to add vertices
- [ ] Area displayed while drawing
- [ ] Closes automatically to start point
- [ ] [Customize: Snapping requirements?]

**Priority:** [If area assets] | **Effort:** Medium

---

#### DRW-006: Edit Asset Geometry
> As an asset manager, I want to edit an asset's location or shape, so that I can correct errors.

**Acceptance Criteria:**
- [ ] Drag vertices to adjust
- [ ] Add new vertices if needed
- [ ] Save or cancel changes
- [ ] [Customize: Audit log of changes?]

**Priority:** Must Have | **Effort:** Medium

---

#### DRW-007: Move Asset
> As an asset manager, I want to move an asset to a new location, so that I can correct placement.

**Acceptance Criteria:**
- [ ] Drag asset to new position
- [ ] Preview shows new location
- [ ] Confirm or cancel move

**Priority:** Should Have | **Effort:** Small

---

#### DRW-008: Delete Asset
> As an asset manager, I want to delete an asset, so that I can remove retired or incorrect entries.

**Acceptance Criteria:**
- [ ] Delete option for authorized users
- [ ] Confirmation required
- [ ] [Customize: Soft delete with reason? Archive?]

**Priority:** Must Have | **Effort:** Small

---

#### DRW-009: Snap to Features
> As an asset manager, I want new assets to snap to existing features, so that I maintain topological accuracy.

**Acceptance Criteria:**
- [ ] Snap to existing vertices
- [ ] Snap to edges
- [ ] Snapping can be toggled
- [ ] Visual indicator when snapping

**Priority:** Should Have | **Effort:** Medium

---

### Search

#### SRC-001: Search for Assets
> As an asset manager, I want to search for an asset by ID or address, so that I can quickly find specific assets.

**Acceptance Criteria:**
- [ ] Search by asset ID
- [ ] Search by address/location
- [ ] Autocomplete suggestions
- [ ] Select result zooms to asset

**Priority:** Must Have | **Effort:** Medium

---

### Styling

#### STY-001: Style by Asset Type
> As an asset manager, I want assets colored by type, so that I can distinguish different asset categories.

**Acceptance Criteria:**
- [ ] Color coding: [type 1 = color 1, type 2 = color 2, ...]
- [ ] Legend shows type-color mapping
- [ ] [Customize: Also style by status?]

**Priority:** Must Have | **Effort:** Medium

---

#### STY-002: Display Asset Icons
> As an asset manager, I want recognizable icons for assets, so that I can identify types at a glance.

**Acceptance Criteria:**
- [ ] Icon for [type 1]: [description]
- [ ] Icon for [type 2]: [description]
- [ ] Icons are clear at typical zoom levels
- [ ] [Customize: Add all asset type icons]

**Priority:** Should Have | **Effort:** Medium

---

#### STY-003: Display Asset Labels
> As an asset manager, I want to see asset labels, so that I can identify specific assets without clicking.

**Acceptance Criteria:**
- [ ] Label shows [asset ID / name / ...]
- [ ] Labels appear at zoom level [X] and higher
- [ ] Labels don't overlap excessively

**Priority:** Should Have | **Effort:** Medium

---

### Controls

#### CTL-001: Display Zoom Buttons
> As an asset manager, I want zoom buttons, so that I have obvious zoom controls.

**Acceptance Criteria:**
- [ ] Zoom in/out buttons visible
- [ ] Positioned [top-right / specify]

**Priority:** Must Have | **Effort:** Small

---

#### CTL-002: Display Scale Bar
> As an asset manager, I want a scale bar, so that I can understand distances.

**Acceptance Criteria:**
- [ ] Scale in [metric / imperial / both]
- [ ] Updates with zoom level

**Priority:** Should Have | **Effort:** Small

---

### Data Management

#### DAT-001: Import Asset Data
> As an asset manager, I want to import assets from a file, so that I can bulk-load data.

**Acceptance Criteria:**
- [ ] Support formats: [CSV, GeoJSON, Shapefile, ...]
- [ ] Validate data before import
- [ ] Report errors and successes
- [ ] [Customize: Field mapping UI?]

**Priority:** Should Have | **Effort:** Medium

---

#### DAT-002: Show Data Freshness
> As an asset manager, I want to know when data was last updated, so that I can trust its accuracy.

**Acceptance Criteria:**
- [ ] Show "last updated" date for each layer
- [ ] Indicate stale data (older than [X days])
- [ ] [Customize: Auto-refresh options?]

**Priority:** Should Have | **Effort:** Small

---

#### DAT-003: Export Asset Data
> As an asset manager, I want to export assets to a file, so that I can use the data in other systems.

**Acceptance Criteria:**
- [ ] Export formats: [CSV, GeoJSON, Shapefile, ...]
- [ ] Export visible or filtered assets
- [ ] Include all attributes

**Priority:** Should Have | **Effort:** Medium

---

### Authentication & Administration

#### ITG-003: Authenticate Users
> As an asset manager, I want to log in, so that I can access the system with my permissions.

**Acceptance Criteria:**
- [ ] Login with [username/password, SSO, ...]
- [ ] Session timeout: [X minutes]
- [ ] Logout option available

**Priority:** Must Have | **Effort:** Large

---

#### ADM-002: Manage User Permissions
> As an administrator, I want to manage user roles, so that I can control who can view and edit assets.

**Acceptance Criteria:**
- [ ] Roles: [viewer, editor, admin]
- [ ] Assign roles to users
- [ ] Role determines capabilities
- [ ] [Customize: Layer-level permissions?]

**Priority:** Must Have | **Effort:** Large

---

### Error Handling & Performance

#### ERR-001: Display Error Messages
> As an asset manager, I want clear errors, so that I know when something fails.

**Acceptance Criteria:**
- [ ] Errors in plain language
- [ ] Suggest next steps
- [ ] Can be dismissed

**Priority:** Must Have | **Effort:** Small

---

#### PRF-001: Fast Initial Load
> As an asset manager, I want the map to load quickly, so that I can start working without delay.

**Acceptance Criteria:**
- [ ] Interactive within [X] seconds
- [ ] Progressive loading of assets
- [ ] Loading indicator during fetch

**Priority:** Must Have | **Effort:** Medium

---

## Customization Checklist

Before using this kit, fill in:

- [ ] Asset types to manage
- [ ] Key attributes for each asset type
- [ ] Required fields for new assets
- [ ] Symbology and icons per type
- [ ] Status values and color coding
- [ ] User roles and permissions
- [ ] Integration points (work orders, ERP, etc.)
- [ ] Data import/export requirements
- [ ] Audit and versioning needs

## Related Resources

- [Asset Management Archetype](../../by-archetype/asset-management.md) - Full archetype guide
- [MVP Checklist](../mvp-checklist.md) - Minimum requirements
- [Dependency Graph](../../dependencies/dependency-graph.md) - Story dependencies
