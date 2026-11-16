**User Story:** As a platform operator, I want to meter usage per tenant, so that
billing reflects actual consumption (NIST Measured Service).

**Acceptance Criteria:**
- Given activity across tenants
- When usage is recorded
- Then metrics are attributable to the correct tenant_id

**Technical Tasks (checklist):**
- [ ] Emit usage metrics tagged by tenant_id
- [ ] Prometheus/Grafana dashboard per tenant
- [ ] Link to nist-mapping.md

**Label:** user-story
