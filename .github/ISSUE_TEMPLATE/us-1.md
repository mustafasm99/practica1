**User Story:** As a customer agent, I want to create a support ticket, so that
I can log a customer issue for tracking.

**Acceptance Criteria:**
- Given an authenticated agent of tenant A
- When they submit a ticket with subject and description
- Then the ticket is stored and its tenant_id is set to A (from the JWT, not the request body)

**Technical Tasks (checklist):**
- [ ] POST /tickets endpoint
- [ ] Extract tenant_id from JWT context
- [ ] Persist with forced tenant filter (RLS)
- [ ] Unit test + isolation test
- [ ] Update API docs

**Label:** user-story
