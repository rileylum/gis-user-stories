# Integration Stories

Sharing, embedding, authentication, and API access.

---

## ITG-001: Share Map View

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Public User, Viewer, Analyst |
| **Archetypes** | Public Portal, Data Viewer, Analysis Tool |
| **Dependencies** | IMP-005 |
| **Effort** | Small |

**User Story:**
> As a map user, I want to share my current map view with others, so that they can see exactly what I'm looking at.

**Acceptance Criteria:**
- [ ] Share button is prominently displayed
- [ ] Clicking share generates a shareable link
- [ ] User can copy the link to clipboard with one click
- [ ] Social sharing options are available (email, Twitter, Facebook)
- [ ] Shared link opens the same map view for recipients
- [ ] _[Customize: Social platforms and share options]_

**Variations:**
- QR code generation for mobile sharing
- Embed code for websites (see ITG-002)
- Share via native mobile share sheet
- Preview of shared content before sharing

**Customization Prompts:**
- Which social sharing platforms should be supported?
- Should QR codes be generated?
- Should there be a preview before sharing?
- What branding should appear in social previews (Open Graph)?

**Non-Functional Considerations:**
- **Performance**: Link generation should be instant
- **Accessibility**: Share button and options must be keyboard accessible
- **Mobile**: Native share sheet integration for better UX

**Related Stories:** IMP-005, ITG-002

---

## ITG-002: Embed Map in Website

| Attribute | Value |
|-----------|-------|
| **Tier** | Enhanced |
| **Personas** | Administrator, Analyst |
| **Archetypes** | Public Portal, Data Viewer |
| **Dependencies** | ITG-001 |
| **Effort** | Medium |

**User Story:**
> As a website administrator, I want to embed the map in my website, so that visitors can interact with it directly.

**Acceptance Criteria:**
- [ ] Embed code (iframe) can be generated
- [ ] User can customize embed size
- [ ] User can select which controls to show in embedded view
- [ ] Embedded map works on third-party websites
- [ ] Embed code can be copied with one click
- [ ] _[Customize: Allowed domains and embed options]_

**Variations:**
- Responsive embed (adjusts to container)
- Static snapshot embed (image)
- Limit features in embedded view
- Custom styling for embedded maps

**Customization Prompts:**
- What embed sizes should be offered?
- Should any controls be hidden in embedded mode?
- Are there domain restrictions for embedding?
- Should embedded maps have limited interactivity?

**Non-Functional Considerations:**
- **Performance**: Embedded maps should load quickly
- **Accessibility**: Embedded map should remain accessible
- **Mobile**: Responsive embeds should work in mobile browsers

**Related Stories:** ITG-001, ITG-004

---

## ITG-003: Authenticate Users

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Viewer, Contributor, Analyst, Field Worker, Administrator |
| **Archetypes** | All (except fully public) |
| **Dependencies** | None |
| **Effort** | Large |

**User Story:**
> As a user, I want to log in to the application, so that I can access features and data according to my permissions.

**Acceptance Criteria:**
- [ ] Login form accepts username/email and password
- [ ] User receives appropriate error messages for failed login
- [ ] Successful login redirects to the application
- [ ] Session persists until logout or timeout
- [ ] Logout option is available
- [ ] _[Customize: Authentication method and session duration]_

**Variations:**
- Social login (Google, Microsoft, GitHub)
- Single Sign-On (SSO) integration
- Multi-factor authentication (MFA)
- Passwordless login (magic link)

**Customization Prompts:**
- What authentication methods should be supported?
- What is the session timeout duration?
- Is single sign-on required?
- Is multi-factor authentication needed?

**Non-Functional Considerations:**
- **Performance**: Login should complete quickly
- **Accessibility**: Login forms must be fully accessible
- **Mobile**: Mobile login experience (biometrics, saved credentials)

**Related Stories:** ITG-004, ADM-002

---

## ITG-004: Access via API

| Attribute | Value |
|-----------|-------|
| **Tier** | Specialized |
| **Personas** | Analyst, Administrator |
| **Archetypes** | Integration, Analysis Tool |
| **Dependencies** | ITG-003 |
| **Effort** | X-Large |

**User Story:**
> As a developer, I want to access map data via an API, so that I can integrate it with other systems.

**Acceptance Criteria:**
- [ ] RESTful API endpoints are available for data access
- [ ] API authentication (API key or OAuth) is supported
- [ ] Documentation describes available endpoints and parameters
- [ ] Standard data formats are supported (GeoJSON, JSON)
- [ ] Rate limiting prevents abuse
- [ ] _[Customize: Available endpoints and authentication method]_

**Variations:**
- GraphQL API in addition to REST
- Real-time data streaming (WebSockets)
- Webhooks for change notifications
- Bulk data export endpoints

**Customization Prompts:**
- What operations should the API support (read, write, both)?
- What authentication method should be used?
- What rate limits are appropriate?
- Should webhooks or real-time updates be supported?

**Non-Functional Considerations:**
- **Performance**: API should be fast and scalable
- **Accessibility**: API documentation should be accessible
- **Mobile**: API should work well for mobile app development

**Related Stories:** ITG-003, DAT-001, DAT-003

---

## Summary

| ID | Story | Tier | Effort |
|----|-------|------|--------|
| ITG-001 | Share Map View | Standard | Small |
| ITG-002 | Embed Map in Website | Enhanced | Medium |
| ITG-003 | Authenticate Users | Standard | Large |
| ITG-004 | Access via API | Specialized | X-Large |
