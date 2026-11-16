**User Story:** As a customer agent, I want to be notified when a ticket is assigned,
so that I can respond quickly without polling.

**Acceptance Criteria:**
- Given a ticket assignment event
- When the event is emitted to the message broker (tagged with tenant_id)
- Then the notifications service sends the notification to the correct tenant only

**Technical Tasks (checklist):**
- [ ] Publish event to message broker
- [ ] Notifications consumer tagged by tenant_id
- [ ] Async test (no blocking of the request path)
- [ ] Update ADR-0006

**Label:** user-story
     