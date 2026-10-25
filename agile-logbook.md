---
title: Agile Logbook
permalink: /agile-logbook/
---

[← Back to portfolio]({{ '/' | relative_url }})

# Agile Logbook – Industry Placement

This logbook documents selected experiences from my software engineering placement at AAG and reflects on how Agile practices relate to planning, communication, implementation, testing, code review, and continuous improvement.

## 1. Daily Logbook Entries

### Entry 1: Investigating Card Management and Points-Account Lookup

**Date:** 04/08/2026

**Work area:** Frontend development and API integration

**Stand-up update:** I was working on improving card-status display and investigating how to retrieve a points account using person and campaign information. My next step was to confirm the expected API behaviour and complete the relevant frontend changes.

**Work completed:** I investigated the existing application flow and worked on displaying card statuses, including active, cancelled, and expired. I also investigated how the application retrieved a points account associated with a person and campaign.

**Next steps:** Verify the API request and response, test relevant scenarios, and address issues identified during review.

**Blockers and dependencies:** Progress depended on understanding the available API functionality, expected parameters, and existing application structure.

**Outcome and learning:** I gained a clearer understanding of how frontend behaviour depends on API contracts and existing application architecture. This showed me the importance of investigating dependencies before committing to an implementation approach.

**Reflection:** I learned that understanding the existing data flow before implementing a solution can prevent unnecessary work. I initially needed to investigate how the application retrieved the required information before deciding on an approach. In future, I would verify the available endpoint, request parameters, and response structure earlier and include this investigation in my task breakdown.

### Entry 2: Validating the Points-Account API Approach

**Date:** 05/08/2026

**Work area:** API integration and implementation refinement

**Stand-up update:** I was investigating the appropriate way to retrieve a points account for a person and campaign. I needed to confirm the available endpoint before finalising the implementation.

**Work completed:** I checked the updated API documentation and identified an endpoint that supported the required lookup. I changed the implementation from relying on frontend filtering to using the appropriate API functionality.

**Next steps:** Verify the returned data and test relevant success and failure scenarios.

**Blockers and dependencies:** The implementation depended on the updated API documentation and the expected request parameters.

**Outcome and learning:** The implementation was better aligned with the backend's intended responsibilities. I also learned how validating an assumption can lead to a more appropriate implementation.

**Evidence:** 
<img src="{{ '/assets/img/data-flow-frontend-to-backend.png' | relative_url }}" alt="Data Flow Frontend to Backend image">

**Reflection:** I initially assumed that filtering data on the frontend was a suitable approach. Checking the API documentation showed that a more appropriate endpoint was available. This taught me to validate technical assumptions before finalising a solution. In future, I would include API-contract verification as an investigation task before breaking the remaining work into implementation and testing tasks.

### Entry 3: Password-Reset Integration and Code Review

**Date:** 01/09/2026

**Work area:** Frontend integration and maintainability

**Stand-up update:** I was connecting the password-reset interface to the existing backend flow and checking that the request and reset steps worked correctly.

**Work completed:** I connected the frontend to the existing one-time password (OTP) request and password-reset functionality. During code review, I received feedback about moving API calls into the application's established model and store layers rather than handling them directly in the UI or controller.

**Next steps:** Apply the review feedback, test the flow again, and verify that the revised implementation follows the existing architecture.

**Blockers and dependencies:** The implementation depended on the existing backend flow and the application's established data-access patterns.

**Outcome and learning:** I gained practical experience integrating existing functionality and responding to architectural feedback. I learned that functional correctness and maintainability are related but distinct aspects of software quality.

**Evidence:**  
<img src="{{ '/assets/img/application-achitecture.png' | relative_url }}" alt="Layered Application Architecture Infographic">

**Reflection:** My initial focus was on connecting the interface to the required functionality. The review feedback helped me recognise that the location of API calls also affects separation of concerns and maintainability. In future, I would examine the existing architectural conventions before implementation and consider both functional requirements and design quality when planning a change.

### Entry 4: Redemption Data and Pagination

**Date:** 02/09/2026

**Work area:** Data retrieval and frontend integration

**Stand-up update:** I was working on displaying redemption information and needed to ensure that the frontend handled the endpoint's response and pagination correctly.

**Work completed:** I worked on retrieving redemption information for the relevant person and campaign, displaying associated information, adapting pagination after an endpoint change, and masking voucher identifiers where required.

**Next steps:** Validate pagination, check empty and unsuccessful responses, and confirm that sensitive identifiers are displayed appropriately.

**Blockers and dependencies:** The work depended on the service response structure and the endpoint's pagination behaviour.

**Outcome and learning:** I developed a better understanding of how backend changes can affect frontend data handling, including pagination, response processing, and the presentation of sensitive information.

**Evidence:** 
<img src="{{ '/assets/img/account-lookup.png' | relative_url }}" alt="Account Lookup Data Flow and Validation Checklist">

**Reflection:** I learned that endpoint changes can affect more than the initial data request. They may also affect how results are processed and displayed. In future, I would verify the response structure and pagination behaviour early, identify relevant edge cases, and include these checks in my task breakdown.

### Entry 5: Catalogue Investigation and Service Integration

**Date:** 15/09/2026

**Work area:** Troubleshooting and application maintenance

**Stand-up update:** I was investigating catalogue-related behaviour and tracing the issue through the relevant code and service dependencies before deciding on a change.

**Work completed:** I investigated catalogue behaviour, replaced a hardcoded catalogue code with a more dynamic approach, and worked on related service and API issues.

**Next steps:** Verify the change against the relevant scenarios and check for regressions.

**Blockers and dependencies:** The investigation depended on understanding the relevant data, application logic, and service behaviour.

**Outcome and learning:** I strengthened my approach to troubleshooting across different application layers and learned to investigate the source of a problem before selecting a solution.

**Evidence:** 
<img src="{{ '/assets/img/troubleshooting-flow.png' | relative_url }}" alt="Troubleshooting Flow Reproduce to Verify">

**Reflection:** I learned not to assume that an issue originates in the frontend simply because it appears there. A visible symptom may have several possible causes. In future, I would reproduce the issue, investigate the relevant dependencies, consider alternative explanations, and test the smallest appropriate change before checking for regressions.

### Entry 6: Automated Testing and Verification

**Date:** 16/09/2026

**Work area:** Automated testing and quality assurance

**Stand-up update:** I was investigating automated test failures and working through the necessary corrections before verifying the changes.

**Work completed:** I investigated Jest test failures, corrected issues, reviewed test coverage, and verified relevant changes.

**Next steps:** Run the relevant tests again, review any remaining failures, and confirm the expected behaviour.

**Blockers and dependencies:** Progress depended on understanding the test failures and the behaviour the tests were intended to verify.

**Outcome and learning:** I gained experience using automated tests to identify problems and assess whether changes preserved expected behaviour. I also recognised the value of considering test scenarios during planning rather than only after implementation.

**Evidence:** 
<img src="{{ '/assets/img/test-plan-validation-checklist.png' | relative_url }}" alt="Test Plan Validation Checklist">

**Reflection:** I learned that testing is more effective when expected behaviour and edge cases are considered during task planning. If testing is left until the end, important scenarios may be overlooked or require additional changes. In future, I would identify relevant test cases when breaking down a user story and use the results to verify that the completed work meets its acceptance criteria.

### Entry 7: Picking-Slip Functionality and PDF Output

**Date:** 01/10/2026

**Work area:** End-to-end application functionality

**Stand-up update:** I was working on picking-slip functionality and needed to verify how the filtering, waybill-related behaviour, and document-generation flow worked together.

**Work completed:** I worked on picking-slip filters, waybill-related functionality, and the flow used to generate and print PDF documents.

**Next steps:** Test the complete workflow, verify the generated document, and check the final browser behaviour.

**Blockers and dependencies:** The workflow involved multiple application layers, so the final output depended on the data, server-side processing, and browser handling working together.

**Outcome and learning:** I gained a better understanding of how a user-facing feature can depend on several connected components and how failures in one part of a workflow can affect the final result.

**Evidence:** <img src="{{ '/assets/img/document-generation-flow.png' | relative_url }}" alt="Document Generation Flow.png">


**Reflection:** I learned that testing an individual component does not necessarily prove that the entire workflow works. A document may be generated successfully but still encounter problems during delivery or printing. In future, I would include an end-to-end validation step that checks the final output from the user's perspective, alongside testing individual components.

## 2. Sprint Retrospective Reflection

### What went well

I gained practical experience investigating existing code, consulting API documentation, implementing changes, correcting automated tests, and responding to code review feedback. These experiences helped me understand how developers maintain and improve established applications. They also showed me the value of investigating a problem before committing to a solution.

### What was challenging

Understanding an existing codebase required me to learn its architecture, service contracts, and dependencies before making changes. API changes and review feedback sometimes required additional investigation or implementation revisions. These experiences showed me that an initial assumption can influence both the implementation and the amount of rework required.

### What I learned

I learned that software development involves more than completing an initial implementation. Understanding requirements, validating assumptions, communicating uncertainty, testing edge cases, and incorporating review feedback all contribute to the quality of the final result.

I also recognised the connection between technical work and Agile planning. Breaking a feature into investigation, implementation, and verification tasks makes the work clearer and helps identify dependencies earlier.

### What I will improve

I want to investigate requirements and API contracts earlier, break work into clearer implementation and testing tasks, and communicate progress and blockers more specifically during stand-ups.

I will assess my improvement by looking for clearer task breakdowns, earlier identification of dependencies, more complete testing of relevant scenarios, and fewer avoidable changes caused by unverified assumptions.

## 3. Overall Reflection

My industry placement has helped me understand how Agile practices support software development as an ongoing team process. Sprint planning helps establish the work to be undertaken, daily stand-ups support coordination, code reviews provide opportunities to improve implementation quality, and retrospectives encourage continuous improvement.

I have learned that communicating specific progress and uncertainties is more useful than giving vague status updates. Explaining what I have investigated, what has changed, what needs to happen next, and what assistance I require helps others understand the status of my work.

My technical experiences have also shown me the importance of connecting planning with implementation and verification. Investigating API contracts, understanding existing architecture, and identifying test scenarios before implementation can help reduce avoidable rework and improve maintainability.

Going forward, I want to become more deliberate about validating assumptions, identifying dependencies before implementation, and including testing and review in my task planning. These practices will help me become a more independent developer while continuing to learn from feedback and team collaboration.