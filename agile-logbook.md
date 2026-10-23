---
title: Agile Logbook
permalink: /agile-logbook/
---

[← Back to portfolio]({{ '/' | relative_url }})

# Agile Logbook – Industry Placement

## 1. Purpose and context

This logbook documents my learning and development as a Software Engineering Intern working in an enterprise software development environment. It focuses on the relationship between daily team communication, sprint planning, implementation, testing, code review, and continuous improvement.

Our team works in two-week sprints. Daily stand-ups take place at 09:15, where team members communicate recent progress, current work, and blockers. Sprint planning takes place at the beginning of each sprint, while completed work is demonstrated and the team reflects on its process at the end of the sprint.

## 2. Daily logbook entries

### Entry 1: Investigating card management and points-account lookup

**Date:** 04/08/2026

**Work area:** Frontend development and API integration

**Stand-up update :** I was working on improving card-status display and the process for finding a points account using person and campaign information. My next step was to confirm the expected API behaviour and complete the relevant frontend changes.

**Work completed:** I investigated the existing application flow and worked on displaying card statuses such as active, cancelled, and expired. I also investigated how the application retrieved a points account associated with a person and campaign.

**Next steps:** Verify the API request and response, test relevant scenarios, and address any issues identified during review.

**Blockers and dependencies:** The implementation depended on understanding the available API functionality and its expected parameters.

**Outcome:** I gained a clearer understanding of how frontend behaviour depends on API contracts and existing application structure.

**Evidence:** Student-created user story, acceptance criteria, and an anonymised task breakdown.

**Reflection:** I learned that understanding the existing data flow before implementing a solution can prevent unnecessary work. In future, I would verify the available endpoint and expected response structure before deciding how to retrieve the data.

### Entry 2: Validating the points-account API approach

**Date:** 05/08/2026

**Work area:** API integration and implementation refinement

**Stand-up update:** I was investigating the appropriate way to retrieve a points account for a person and campaign. I needed to confirm the available endpoint before finalising the implementation.

**Work completed:** I checked the updated API documentation and identified an endpoint that supported the required lookup. I changed the implementation from relying on frontend filtering to using the appropriate API functionality.

**Next steps:** Verify the returned data and test the relevant success and failure scenarios.

**Blockers and dependencies:** The implementation depended on the updated API documentation and the expected request parameters.

**Outcome:** The implementation was aligned more closely with the backend's intended responsibilities.

**Evidence:** An anonymised implementation flow showing the frontend request, API lookup, and returned result.

**Reflection:** I initially assumed that filtering data on the frontend was a suitable approach. Checking the API documentation showed that a more appropriate endpoint was available. Next time, I would investigate the API contract before selecting an implementation strategy and breaking the work into tasks.

### Entry 3: Password-reset integration and code review

**Date:** 01/09/2026

**Work area:** Frontend integration and maintainability

**Stand-up update:** I was connecting the password-reset interface to the existing backend flow and checking that the request and reset steps worked correctly.

**Work completed:** I connected the frontend to the existing OTP request and password-reset functionality. During code review, I received feedback about moving API calls into the application's established models and stores rather than handling them directly in the UI or controller.

**Next steps:** Apply the review feedback, test the flow again, and verify that the revised implementation follows the existing architecture.

**Blockers and dependencies:** The implementation depended on the existing backend flow and the application's established data-access patterns.

**Outcome:** I gained practical experience integrating existing functionality and responding to architectural feedback.

**Evidence:** A self-created diagram showing the separation between the UI, model/store layer, and backend service.

**Reflection:** This experience taught me that a feature can work functionally while still requiring improvements to maintainability. In future, I would examine existing architectural conventions before implementing API integration.

### Entry 4: Redemption data and pagination

**Date:** 02/09/2026

**Work area:** Data retrieval and frontend integration

**Stand-up update:** I was working on displaying redemption information and needed to ensure that the frontend handled the endpoint's response and pagination correctly.

**Work completed:** I worked on retrieving redemption information for the relevant person and campaign, displaying associated information, adapting pagination after an endpoint change, and masking voucher identifiers where required.

**Next steps:** Validate pagination, check empty and unsuccessful responses, and confirm that sensitive identifiers are displayed appropriately.

**Blockers and dependencies:** The work depended on the service response structure and the endpoint's pagination behaviour.

**Outcome:** I developed a better understanding of how backend changes can affect frontend data handling.

**Evidence:** An anonymised data-flow diagram and a student-created validation checklist.

**Reflection:** I learned that endpoint changes can affect more than the initial data request. In future, I would verify the response structure and pagination behaviour early and include representative test scenarios in my task breakdown.

### Entry 5: Catalogue investigation and service integration

**Date:** 15/09/2026

**Work area:** Troubleshooting and application maintenance

**Stand-up update:** I was investigating catalogue-related behaviour and tracing the issue through the relevant code and service dependencies before deciding on a change.

**Work completed:** I investigated catalogue behaviour, replaced a hardcoded catalogue code with a more dynamic approach, and worked on related service/API issues.

**Next steps:** Verify the change against the relevant scenarios and check for regressions.

**Blockers and dependencies:** The investigation depended on understanding the relevant data, application logic, and service behaviour.

**Outcome:** I strengthened my approach to troubleshooting problems across different application layers.

**Evidence:** A self-created troubleshooting flow showing reproduction, investigation, implementation, and verification.

**Reflection:** I learned not to assume that an issue originates in the frontend simply because it appears there. In future, I would reproduce the problem, inspect the relevant dependencies, and test the smallest appropriate change.

### Entry 6: Automated testing and verification

**Date:** 16/09/2026

**Work area:** Automated testing and quality assurance

**Stand-up update :** I was investigating automated test failures and working through the necessary corrections before verifying the changes.

**Work completed:** I investigated Jest test failures, corrected issues, reviewed test coverage, and verified relevant changes.

**Next steps:** Run the relevant tests again, review any remaining failures, and confirm the expected behaviour.

**Blockers and dependencies:** Progress depended on understanding the test failures and the behaviour the tests were intended to verify.

**Outcome:** I gained experience using automated tests to identify problems and check whether changes preserved expected behaviour.

**Evidence:** A portfolio-safe test checklist or an original example test plan that contains no proprietary code or internal data.

**Reflection:** I learned that testing is more effective when expected behaviour and edge cases are considered during task planning. Next time, I would identify important scenarios before implementation rather than leaving test planning until the end.

### Entry 7: Picking-slip functionality and PDF output

**Date:** 01/10/2026

**Work area:** End-to-end application functionality

**Stand-up update:** I was working on picking-slip functionality and needed to verify how the filtering, waybill-related behaviour, and document-generation flow worked together.

**Work completed:** I worked on picking-slip filters, waybill-related functionality, and the flow used to generate and print PDF documents.

**Next steps:** Test the complete workflow, verify the generated document, and check the final browser behaviour.

**Blockers and dependencies:** The workflow involved multiple application layers, so successful output depended on the data, server-side processing, and browser handling working together.

**Outcome:** I gained a better understanding of how a user-facing feature can depend on several connected components.

**Evidence:** A self-created diagram illustrating a generic document-generation workflow from input data to browser output.

**Reflection:** I learned that testing an individual component does not necessarily prove that the entire workflow works. In future, I would include an end-to-end validation step that checks the final output from the user's perspective.

## 3. Sprint retrospective reflection

_This section summarises learning across my placement experiences. It is not a verbatim record of a particular sprint retrospective._

### What went well

I gained practical experience investigating existing code, consulting API documentation, implementing changes, writing and correcting tests, and responding to code review feedback. These activities helped me understand how developers maintain and improve established applications.

### What was challenging

Understanding an existing codebase required me to learn its architecture, service contracts, and dependencies before making changes. API changes and review feedback sometimes required further investigation or implementation revisions.

### What I learned

I learned that software development involves more than completing an initial implementation. Understanding requirements, validating assumptions, communicating uncertainty, testing edge cases, and incorporating review feedback all contribute to the quality of the final result.

### What I will improve

I want to investigate requirements and API contracts earlier, break work into clearer implementation and testing tasks, and communicate progress and blockers more specifically during stand-ups.

I will assess my improvement by looking for clearer task breakdowns, earlier identification of dependencies, more complete testing of relevant scenarios, and fewer avoidable changes caused by assumptions about existing functionality.

## 4. Overall reflection

My industry placement has helped me understand how Agile practices support software development as an ongoing team process. Sprint planning helps the team agree on intended work, daily stand-ups support coordination, code reviews provide opportunities to improve implementation quality, and retrospectives encourage continuous improvement.

I have learned that communicating specific progress and uncertainties is more useful than giving vague status updates. Explaining what I have investigated, what has changed, what needs to happen next, and what assistance I require helps the team coordinate its work.

Going forward, I want to become more deliberate about validating assumptions, identifying dependencies before implementation, and including testing and review in my task planning. These practices will help me become a more independent developer while continuing to learn from the team's experience.

## 5. Evidence

The following portfolio-safe artefacts support the learning described in this logbook:

1. **Two-week sprint timeline:** A self-created diagram illustrating sprint planning, daily stand-ups, development, a sprint demonstration, and a retrospective.
    
2. **Development work summary:** An anonymised example connecting a user story to investigation, implementation, testing, and review.
    
3. **Testing and validation checklist:** A self-created checklist showing how expected behaviour, edge cases, and unsuccessful responses can be verified.
    
4. **Personal learning record:** Reflections on genuine technical challenges, code review feedback, and improvements to my development process.

---

[← Back to portfolio]({{ '/' | relative_url }})
