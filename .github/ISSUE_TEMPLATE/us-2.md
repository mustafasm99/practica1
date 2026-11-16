**User Story:** As a customer agent, I want to see only my tenant's tickets, so that
I never see another company's data.

**Acceptance Criteria:**
- Given a token for tenant A
- When they request the ticket list
- Then only tickets with tenant_id = A are returned; tenant B tickets are never
  included, even if IDs are guessed

**Technical Tasks (checklist):**
- [ ] GET /tickets with tenant filter
- [ ] Enforce via RLS policy
- [ ] Isolation test: tenant A cannot read tenant B tickets
- [ ] Update API docs

**Label:** user-story
