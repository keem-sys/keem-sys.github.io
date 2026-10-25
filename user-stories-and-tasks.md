---
title: User Stories and Tasks
permalink: /user-stories-and-tasks/
---

[← Back to portfolio]({{ '/' | relative_url }})

# User Stories and Tasks - Industry Placement

## Story 1 - View card status accurately

**User story:** As a banking application user, I want to see a card's current status so that I can understand whether it can be used.

**Acceptance criteria**
- The interface displays the status returned by the appropriate service.
- Active, cancelled, and expired cards are handled consistently with the agreed business rules.
- Empty or unexpected responses do not cause the screen to fail.
- The behaviour is tested against relevant API responses.

**Tasks**
1. Review the existing card-management UI and data flow.
2. Confirm the source of card status and relevant API contract.
3. Implement or update the status filtering/display logic.
4. Test active, cancelled, expired, and empty-result cases.
5. Verify the change and document the outcome in the ticket.

**Placement connection:** Work included a card popup that filtered active/cancelled/expired cards and UI changes that were demonstrated to a mentor for feedback.

## Story 2 - Find points accounts by person and campaign

**User story:** As an authorised user, I want to retrieve the correct points account for a person and campaign so that the application displays the relevant account information.

**Acceptance criteria**
- The request uses the agreed person and campaign identifiers.
- The implementation follows the documented API contract.
- No client-side filtering workaround is used when the service endpoint is intended to perform the lookup.
- Missing or unsuccessful results are handled appropriately.

**Tasks**
1. Inspect the existing frontend filtering and API call.
2. Confirm the endpoint and parameters against the banking API specification.
3. Replace the local filtering approach with the service lookup where appropriate.
4. Test valid, missing, and unsuccessful responses.
5. Submit the change for review and incorporate feedback.

**Placement connection:** The implementation was changed to call the relevant points-account endpoint after the API documentation was updated.

## Story 3 - Reset a user's password through the existing service

**User story:** As a user who cannot access my account, I want to request an OTP and reset my password so that I can regain access securely.

**Acceptance criteria**
- The UI calls the existing backend flow rather than duplicating business logic in the frontend.
- OTP request and password reset responses are handled clearly.
- Loading and error states are understandable.
- The implementation follows the established model/store/controller conventions and is reviewed.

**Tasks**
1. Trace the current frontend-to-backend flow.
2. Connect the request-OTP and reset-password interactions.
3. Test the successful flow and relevant failure cases.
4. Move API calls into the appropriate models/stores in response to review feedback.
5. Re-test and submit the revised implementation.

**Placement connection:** The frontend was connected to an existing backend password-reset flow, and review feedback prompted a change to where API calls were placed.

## Story 4 - View redemptions for a person and campaign

**User story:** As an authorised business user, I want to view redemptions associated with a person and campaign so that I can inspect relevant voucher transactions.

**Acceptance criteria**
- The correct person and campaign context is passed to the service.
- Returned redemptions and their items/transactions are displayed consistently.
- Pagination works with the current endpoint contract.
- Voucher identifiers are masked where required.
- Errors and empty results are handled.

**Tasks**
1. Trace the person/campaign selection and redemption API flow.
2. Connect the relevant service response to the grid and detail views.
3. Adapt pagination after the endpoint changed.
4. Apply masking to voucher numbers where required.
5. Test representative responses and submit for review.

**Placement connection:** Work included a person-and-campaign redemption flow, pagination changes, and masked voucher numbers.

## Story 5 - Improve catalogue reliability

**User story:** As a user of the catalogue application, I want catalogue data and rules to be handled consistently so that I can use the catalogue without avoidable errors.

**Acceptance criteria**
- The implementation follows the current service/API contract.
- Rules that should be data-driven are not unnecessarily hardcoded.
- Empty responses and expected errors are handled.
- Relevant tests pass and staging behaviour is verified where required.

**Tasks**
1. Reproduce the issue and inspect the relevant logs/code path.
2. Confirm the expected catalogue code or section mapping with the appropriate source.
3. Implement the focused fix.
4. Add or update tests.
5. Verify the result and record the evidence.

**Placement connection:** Internship work included replacing a hardcoded catalogue code with a dynamic approach, addressing catalogue-related API issues, and verifying fixes.

## Story 6 - Produce picking-slip output reliably

**User story:** As an authorised operational user, I want to generate and print a picking slip so that warehouse processing can use the correct document.

**Acceptance criteria**
- The selected warehouse and picking-slip status filters are applied as expected.
- The document uses the intended layout and data.
- The generated PDF is delivered to the browser in a valid binary format.
- Print behaviour is tested in the target workflow.

**Tasks**
1. Confirm the relevant filters and expected default selection.
2. Trace the data-to-PDF flow.
3. Verify PDF buffer/base64 handling between the service and browser.
4. Adapt the document layout to the approved design.
5. Test generation, display, and print behaviour.

**Placement connection:** Work included picking-slip filters, waybill updates, and tracing a PDF generation flow from server-side output to browser printing.

## Story 7 - Maintain automated test reliability

**User story:** As a developer on the team, I want automated tests to reflect expected service behaviour so that regressions are detected before changes are integrated.

**Acceptance criteria**
- Tests cover the relevant expected behaviour and important failure cases.
- Test setup and assertions match the current implementation.
- Tests run successfully in the intended environment.
- Failures are investigated rather than bypassed.

**Tasks**
1. Run the relevant test suite and identify failures.
2. Compare failures with the current implementation and test documentation.
3. Correct outdated assumptions or implementation defects.
4. Re-run the suite and review coverage where available.
5. Record the result and submit changes for review.

**Placement connection:** Work included Jest tests, fixing failing tests, reviewing coverage, and staging verification.

## Personal Reflection

While working on the points-account lookup feature, I initially assumed that filtering the available data on the frontend was an acceptable way to retrieve the account associated with a particular person and campaign. I later validated this approach by checking the updated banking API documentation and confirming that an endpoint was available to perform the lookup directly using the relevant identifiers.

Based on this, I changed the implementation to call the appropriate service endpoint instead of relying on client-side filtering. This taught me the importance of understanding the available API functionality before deciding how to implement a user story. Although a frontend workaround may appear to solve the immediate problem, using the intended endpoint can reduce unnecessary processing and keep the implementation aligned with the backend's responsibilities.

Next time, I would review the API documentation and confirm the expected request parameters and response structure before breaking the story into development tasks. I would also include explicit tasks for validating the API contract and testing successful, missing, and unsuccessful responses. This would help me make better implementation decisions earlier, reduce avoidable rework, and produce a more reliable solution.

## Evidence

1. User story breakdown diagram of points account lookup
<img src="{{ '/assets/img/user-story-breakdown.png' | relative_url }}" alt="Points account lookup story breakdown.png">
   

2. User story-to-task traceability table
<img src="{{ '/assets/img/traceability_table.png' | relative_url }}" alt="Points account lookup story breakdown.png">


---

[← Back to portfolio]({{ '/' | relative_url }})
