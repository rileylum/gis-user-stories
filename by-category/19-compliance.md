# Compliance Stories

Regulatory compliance, accessibility standards, and data governance.

---

## CMP-001: WCAG Accessibility Compliance

| Attribute | Value |
|-----------|-------|
| **Tier** | Foundation |
| **Personas** | Public User, Viewer, Contributor, Analyst |
| **Archetypes** | All |
| **Dependencies** | ACC-001, ACC-002, ACC-003 |
| **Effort** | Large |

**User Story:**
> As an administrator, I need the application to meet WCAG 2.1 AA standards, so that we comply with accessibility regulations and serve all users.

**Acceptance Criteria:**
- [ ] All pages pass automated WCAG 2.1 AA testing
- [ ] Manual accessibility audit confirms compliance
- [ ] Keyboard navigation is fully functional
- [ ] Screen reader navigation is effective
- [ ] Color contrast meets minimum ratios (4.5:1 text, 3:1 UI)
- [ ] Accessibility statement is published
- [ ] _[Customize: WCAG level and additional requirements]_

**Variations:**
- WCAG 2.1 AAA compliance
- Section 508 compliance (US federal)
- EN 301 549 compliance (EU)
- Organization-specific accessibility standards

**Customization Prompts:**
- What WCAG compliance level is required (A, AA, AAA)?
- Are there jurisdiction-specific requirements (Section 508, EN 301 549)?
- Should an accessibility statement be published?
- What remediation timeline is needed for issues found?

**Non-Functional Considerations:**
- **Performance**: Accessibility features should not impact performance
- **Accessibility**: This IS the accessibility requirement
- **Mobile**: Mobile accessibility must be included (touch, VoiceOver, TalkBack)

**Related Stories:** ACC-001, ACC-002, ACC-003

---

## CMP-002: Privacy Compliance

| Attribute | Value |
|-----------|-------|
| **Tier** | Standard |
| **Personas** | Administrator |
| **Archetypes** | All |
| **Dependencies** | ITG-003 |
| **Effort** | Medium |

**User Story:**
> As an administrator, I need the application to comply with privacy regulations, so that we protect user data and avoid legal issues.

**Acceptance Criteria:**
- [ ] Privacy policy is published and linked from the application
- [ ] User consent is obtained before collecting personal data
- [ ] Users can request their data (data subject access request)
- [ ] Users can request deletion of their data
- [ ] Data collection is limited to what's necessary
- [ ] Location data handling complies with regulations
- [ ] _[Customize: Applicable privacy regulations]_

**Variations:**
- GDPR compliance (EU)
- CCPA compliance (California)
- PIPEDA compliance (Canada)
- Cookie consent management

**Customization Prompts:**
- What privacy regulations apply (GDPR, CCPA, etc.)?
- What personal data is collected by the application?
- Is location tracking used, and if so, how is consent managed?
- What data retention periods are required?

**Non-Functional Considerations:**
- **Performance**: Privacy features should not impact user experience
- **Accessibility**: Consent dialogs must be accessible
- **Mobile**: Consent flows must work well on mobile

**Related Stories:** ITG-003, LOC-001, LOC-002

---

## CMP-003: Data Governance

| Attribute | Value |
|-----------|-------|
| **Tier** | Specialized |
| **Personas** | Administrator |
| **Archetypes** | Asset Management, Collaborative Editor, Analysis Tool |
| **Dependencies** | ADM-002, DAT-004 |
| **Effort** | Large |

**User Story:**
> As an administrator, I need data governance controls, so that we maintain data quality, security, and regulatory compliance.

**Acceptance Criteria:**
- [ ] Data classification system identifies sensitive data
- [ ] Access controls limit who can view/edit sensitive data
- [ ] Audit logs track all data access and modifications
- [ ] Data retention policies are enforced
- [ ] Data lineage/provenance is tracked
- [ ] Compliance reports can be generated
- [ ] _[Customize: Governance policies and classifications]_

**Variations:**
- Automated data classification
- Data quality scoring
- Compliance dashboards
- Third-party compliance integrations

**Customization Prompts:**
- What data classification levels are needed?
- What audit logging is required?
- What retention policies must be enforced?
- Are compliance reports needed for specific regulations?

**Non-Functional Considerations:**
- **Performance**: Governance checks should not slow operations
- **Accessibility**: Governance interfaces must be accessible
- **Mobile**: Core governance is typically desktop; mobile should respect classifications

**Related Stories:** ADM-002, DAT-004, ITG-003, CMP-002

---

## Summary

| ID | Story | Tier | Effort |
|----|-------|------|--------|
| CMP-001 | WCAG Accessibility Compliance | Foundation | Large |
| CMP-002 | Privacy Compliance | Standard | Medium |
| CMP-003 | Data Governance | Specialized | Large |
