# User Story Template

Use this template when creating new user stories for the repository.

---

## Template

```markdown
### [PREFIX]-[###]: [Title]

| Attribute | Value |
|-----------|-------|
| **Tier** | [Foundation / Standard / Enhanced / Specialized] |
| **Personas** | [List applicable personas] |
| **Archetypes** | [List applicable archetypes] |
| **Dependencies** | [Story IDs or "None"] |
| **Effort** | [Small / Medium / Large / X-Large] |

**User Story:**
> As a [role], I want to [action], so that [benefit].

**Acceptance Criteria:**
- [ ] [Specific, testable criterion]
- [ ] [Specific, testable criterion]
- [ ] _[Customize: Question for project-specific decision]_

**Variations:**
- [Alternative implementation or use case]
- [Alternative implementation or use case]

**Customization Prompts:**
- [Question to help tailor this story]
- [Question to help tailor this story]

**Non-Functional Considerations:**
- **Performance**: [Performance requirements or considerations]
- **Accessibility**: [Accessibility requirements]
- **Mobile**: [Mobile/responsive considerations]

**Related Stories:** [Comma-separated list of related story IDs]
```

---

## Guidelines

### Story ID

Use the appropriate prefix for the category and a sequential three-digit number:

| Category | Prefix |
|----------|--------|
| Navigation | NAV |
| Layer Management | LAY |
| Data Display | DIS |
| Feature Interaction | INT |
| Drawing & Editing | DRW |
| Measurement | MEA |
| Location Services | LOC |
| Search & Geocoding | SRC |
| Controls & UI | CTL |
| Import & Export | IMP |
| Styling | STY |
| Projections | PRJ |
| Accessibility | ACC |
| Data Management | DAT |
| Integration | ITG |
| Administration | ADM |
| Performance | PRF |
| Error Handling | ERR |
| Compliance | CMP |

### Tiers

- **Foundation**: Essential for any map application. Core functionality.
- **Standard**: Common features that most applications include.
- **Enhanced**: Advanced features that improve user experience.
- **Specialized**: Domain-specific or power-user features.

### Personas

Choose from:
- **Public User**: Anonymous visitor, read-only access
- **Viewer**: Authenticated user, read-only access
- **Contributor**: Can add/edit data
- **Analyst**: Performs spatial analysis
- **Field Worker**: Mobile user collecting data
- **Administrator**: Manages system configuration

### Archetypes

Choose from:
- **Public Portal**: Read-only maps for public consumption
- **Asset Management**: Track and manage physical assets
- **Field Collection**: Mobile data gathering
- **Analysis Tool**: Spatial analysis and decision support
- **Data Viewer**: Internal data visualization
- **Collaborative Editor**: Multi-user map editing

### Effort

- **Small**: ~1-2 days, straightforward implementation
- **Medium**: ~3-5 days, some complexity or dependencies
- **Large**: ~1-2 weeks, significant development effort
- **X-Large**: 2+ weeks, complex feature requiring architecture decisions

### Writing Good Acceptance Criteria

Acceptance criteria should be:
- **Specific**: Clearly defined, no ambiguity
- **Testable**: Can be verified as pass/fail
- **User-focused**: Describe what the user experiences
- **Independent**: Each criterion stands alone

Good examples:
- "User can click and drag to pan the map"
- "Zoom control buttons are visible in the top-right corner"
- "Selected feature is highlighted with a blue outline"

Avoid:
- "The map should work well" (not specific)
- "Performance is good" (not testable)
- "Uses efficient algorithms" (not user-focused)

### Customization Prompts

Include bracketed customization points in acceptance criteria for decisions that vary by project:

```markdown
- [ ] _[Customize: Define the maximum file size for uploads (recommended: 10MB)]_
- [ ] _[Customize: Should layer order be persisted between sessions?]_
```

### Non-Functional Considerations

Always address:
- **Performance**: Response times, data limits, optimization needs
- **Accessibility**: Keyboard operation, screen reader support, WCAG compliance
- **Mobile**: Touch support, responsive design, offline capability

---

## Example

### DRW-010: Undo/Redo Drawing Actions

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Contributor, Analyst, Field Worker |
| **Archetypes** | Field Collection, Collaborative Editor |
| **Dependencies** | DRW-001, DRW-002, DRW-003 |
| **Effort** | Medium |

**User Story:**
> As a map editor, I want to undo and redo my drawing actions, so that I can correct mistakes without starting over.

**Acceptance Criteria:**
- [ ] User can undo the last drawing action using Ctrl+Z or an undo button
- [ ] User can redo an undone action using Ctrl+Y or a redo button
- [ ] Undo/redo history includes at least the last 20 actions
- [ ] _[Customize: Should undo history persist across sessions?]_

**Variations:**
- Step-by-step undo (each vertex is one action)
- Feature-level undo (entire feature is one action)
- Selective undo (choose which actions to undo)

**Customization Prompts:**
- How many actions should be kept in the undo history?
- Should undo history be shared in collaborative editing scenarios?
- Should complex operations (like splitting a polygon) be undone as one action or multiple?

**Non-Functional Considerations:**
- **Performance**: Undo history should not impact memory significantly
- **Accessibility**: Keyboard shortcuts must work; screen readers should announce undo/redo actions
- **Mobile**: Consider touch-friendly undo/redo buttons for mobile devices

**Related Stories:** DRW-001, DRW-002, DRW-003, DRW-004, DRW-007
