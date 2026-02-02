# Web Mapping User Story Repository

A comprehensive collection of user stories for web mapping applications, designed to help Business Analysts, Product Managers, and Development Teams define requirements for GIS and mapping projects.

## Purpose

This repository provides:

- **Pre-written user stories** covering common web mapping functionality
- **Customization prompts** to tailor stories to your specific needs
- **Acceptance criteria** that can be directly converted to test cases
- **Archetype guides** for different types of mapping applications
- **Starter kits** to quickly bootstrap common project types

## How to Use This Repository

### 1. Identify Your Application Archetype

Start with the [archetype guides](by-archetype/) to understand which type of mapping application you're building:

| Archetype | Description | Guide |
|-----------|-------------|-------|
| Public Portal | Read-only maps for public consumption | [public-portal.md](by-archetype/public-portal.md) |
| Asset Management | Track and manage physical assets | [asset-management.md](by-archetype/asset-management.md) |
| Field Collection | Mobile data gathering in the field | [field-collection.md](by-archetype/field-collection.md) |
| Analysis Tool | Spatial analysis and decision support | [analysis-tool.md](by-archetype/analysis-tool.md) |
| Data Viewer | Internal data visualization | [data-viewer.md](by-archetype/data-viewer.md) |
| Collaborative Editor | Multi-user map editing | [collaborative-editor.md](by-archetype/collaborative-editor.md) |

### 2. Use a Starter Kit (Optional)

For common project types, use our [starter kits](quick-start/starter-kits/) which provide a curated set of stories ready to use:

- [Public Portal Starter](quick-start/starter-kits/public-portal-starter.md)
- [Field App Starter](quick-start/starter-kits/field-app-starter.md)
- [Asset Management Starter](quick-start/starter-kits/asset-management-starter.md)

### 3. Browse by Category

Stories are organized into 25 categories:

| # | Category | Stories | Description |
|---|----------|---------|-------------|
| 01 | [Navigation](by-category/01-navigation.md) | 7 | Pan, zoom, rotate, reset |
| 02 | [Layer Management](by-category/02-layer-management.md) | 5 | Toggle, opacity, reorder layers |
| 03 | [Data Display](by-category/03-data-display.md) | 6 | Basemaps, vectors, heatmaps |
| 04 | [Feature Interaction](by-category/04-feature-interaction.md) | 5 | Select, hover, popups |
| 05 | [Drawing & Editing](by-category/05-drawing-editing.md) | 9 | Draw and edit geometries |
| 06 | [Measurement](by-category/06-measurement.md) | 3 | Distance and area tools |
| 07 | [Location Services](by-category/07-location-services.md) | 4 | GPS and geolocation |
| 08 | [Search & Geocoding](by-category/08-search-geocoding.md) | 3 | Address and coordinate search |
| 09 | [Controls & UI](by-category/09-controls-ui.md) | 6 | Zoom buttons, scale bar, etc. |
| 10 | [Import & Export](by-category/10-import-export.md) | 5 | File import, image export |
| 11 | [Styling](by-category/11-styling.md) | 4 | Symbols, labels, colors |
| 12 | [Projections](by-category/12-projections.md) | 3 | Coordinate systems |
| 13 | [Accessibility](by-category/13-accessibility.md) | 3 | Keyboard, screen reader |
| 14 | [Data Management](by-category/14-data-management.md) | 4 | Upload, download, sync |
| 15 | [Integration](by-category/15-integration.md) | 4 | Sharing, embedding, APIs |
| 16 | [Administration](by-category/16-administration.md) | 4 | Config, permissions |
| 17 | [Performance](by-category/17-performance.md) | 4 | Speed, offline, caching |
| 18 | [Error Handling](by-category/18-error-handling.md) | 4 | Errors, retry, recovery |
| 19 | [Compliance](by-category/19-compliance.md) | 3 | WCAG, privacy, governance |
| 20 | [Routing & Directions](by-category/20-routing.md) | 5 | Routes, directions, isochrones |
| 21 | [Geofencing](by-category/21-geofencing.md) | 4 | Zone monitoring, notifications |
| 22 | [Geoprocessing](by-category/22-geoprocessing.md) | 5 | Buffer, intersect, spatial join |
| 23 | [Print & Cartography](by-category/23-print-cartography.md) | 4 | Print layouts, map series |
| 24 | [Charts & Dashboards](by-category/24-charts-dashboards.md) | 4 | Charts, statistics, dashboards |
| 25 | [3D & Terrain](by-category/25-3d-terrain.md) | 3 | 3D terrain, extrusion, navigation |

### 4. Customize Stories for Your Project

Each story includes:

- **Customization prompts**: Questions to adapt the story to your needs
- **Variations**: Alternative implementations to consider
- **Non-functional considerations**: Performance, accessibility, mobile aspects

Copy stories into your project backlog and fill in the bracketed `[Customize: ...]` sections.

### 5. Check Dependencies

Before finalizing your backlog, review the [dependency graph](dependencies/dependency-graph.md) to ensure you've included prerequisite stories.

## Story Tiers

Stories are categorized by implementation priority:

| Tier | Description |
|------|-------------|
| **Foundation** | Essential for any map application |
| **Standard** | Common features most applications need |
| **Enhanced** | Advanced features for richer experiences |
| **Specialized** | Domain-specific or power-user features |

## Effort Estimates

Stories include relative effort estimates:

| Effort | Description |
|--------|-------------|
| **Small** | ~1-2 days, straightforward implementation |
| **Medium** | ~3-5 days, some complexity |
| **Large** | ~1-2 weeks, significant development |
| **X-Large** | 2+ weeks, complex feature |

## Quick Reference

- [Glossary](GLOSSARY.md) - GIS terms explained simply
- [Story Template](STORY-TEMPLATE.md) - Template for writing new stories
- [MVP Checklist](quick-start/mvp-checklist.md) - Essential stories for any project
- [Dependency Graph](dependencies/dependency-graph.md) - Story prerequisites

## Contributing

To add new stories:

1. Use the [Story Template](STORY-TEMPLATE.md)
2. Follow the ID scheme (e.g., NAV-001, LAY-002)
3. Include all required sections
4. Add dependencies to the dependency graph

## ID Scheme Reference

| Category | Prefix | Example |
|----------|--------|---------|
| Navigation | NAV | NAV-001 |
| Layer Management | LAY | LAY-001 |
| Data Display | DIS | DIS-001 |
| Feature Interaction | INT | INT-001 |
| Drawing & Editing | DRW | DRW-001 |
| Measurement | MEA | MEA-001 |
| Location Services | LOC | LOC-001 |
| Search & Geocoding | SRC | SRC-001 |
| Controls & UI | CTL | CTL-001 |
| Import & Export | IMP | IMP-001 |
| Styling | STY | STY-001 |
| Projections | PRJ | PRJ-001 |
| Accessibility | ACC | ACC-001 |
| Data Management | DAT | DAT-001 |
| Integration | ITG | ITG-001 |
| Administration | ADM | ADM-001 |
| Performance | PRF | PRF-001 |
| Error Handling | ERR | ERR-001 |
| Compliance | CMP | CMP-001 |
| Routing & Directions | RTE | RTE-001 |
| Geofencing | GEO | GEO-001 |
| Geoprocessing | GPR | GPR-001 |
| Print & Cartography | PRT | PRT-001 |
| Charts & Dashboards | CHT | CHT-001 |
| 3D & Terrain | 3DT | 3DT-001 |
