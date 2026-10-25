---
title: Product Backlog
permalink: /product-backlog/
---

[← Back to portfolio]({{ '/' | relative_url }})

# Product Backlog – Industry Placement

## 1. Purpose and scope

This product backlog is an independently prepared academic artefact based on my learning and experiences as a Software Engineering Intern at Achievements Awards Group. It summarises types of software development work I encountered during my industry placement without reproducing the company's internal backlog or project management records.

The backlog covers improvements to existing business applications and services, including frontend functionality, API integration, data handling, automated testing, operational workflows, and verification.

The items are anonymised and written for portfolio demonstration.

## 2. Product backlog items

| ID | Backlog item | User/business value | Portfolio priority |
|---|---|---|---|
| PB-01 | Improve card-status display and filtering | Helps users understand whether a card is active, cancelled, or expired. | High |
| PB-02 | Retrieve points accounts using the appropriate API endpoint | Improves the accuracy and maintainability of person-and-campaign account lookups. | High |
| PB-03 | Integrate the password-reset interface with the existing backend | Supports account recovery while keeping API communication within the appropriate application layers. | High |
| PB-04 | Improve redemption retrieval and pagination | Helps authorised users retrieve and navigate redemption records consistently. | High |
| PB-05 | Protect sensitive voucher identifiers in the interface | Reduces unnecessary exposure of sensitive identifiers in relevant views. | High |
| PB-06 | Replace hardcoded catalogue rules with data-driven logic | Reduces fragile assumptions and improves maintainability when catalogue data changes. | Medium |
| PB-07 | Correct catalogue and service integration issues | Improves reliability by aligning application behaviour with API contracts and expected business rules. | High |
| PB-08 | Improve loading, empty, and error states | Helps users understand what is happening when data is unavailable or a request fails. | Medium |
| PB-09 | Maintain and repair automated tests | Helps detect regressions and increases confidence in code changes. | High |
| PB-10 | Improve operational document generation and printing | Supports reliable document generation, display, and printing for operational workflows. | Medium |
| PB-11 | Correct form input and endpoint integration behaviour | Improves input handling and reduces avoidable request failures. | Medium |
| PB-12 | Verify changes and record test outcomes | Helps establish that changes meet requirements and work in the appropriate environment. | High |


## 3. Backlog prioritisation

The suggested priorities consider potential effects on functional correctness, user experience, maintainability, data protection, and regression risk.

Items involving incorrect data retrieval, account recovery, sensitive identifiers, or core functionality are assigned higher illustrative priorities because defects in these areas could have a significant impact. Testing and verification are also important because they help establish confidence that changes have not introduced regressions.

## 4. Backlog refinement and task breakdown

A backlog item should be understood and refined before it is selected for implementation. Depending on the work involved, this may include:

1. Clarifying the user or business problem.
2. Defining expected behaviour and acceptance criteria.
3. Reviewing relevant code, API specifications, and dependencies.
4. Breaking the work into smaller development and testing tasks.
5. Discussing relative complexity during sprint planning and assigning story points.
6. Confirming the expected verification and review requirements.

During my placement, I encountered work that required investigating existing application behaviour, checking API documentation, adapting implementations, addressing review feedback, and verifying changes. These experiences showed me why backlog refinement needs to consider more than coding effort alone.

## 5. Original backlog artefact


### Backlog Summary

| ID | Work category | Deliverable | Priority |
|---|---|---|---|
| A-01 | Investigation | Document the expected account-lookup behaviour and relevant API requirements. | High |
| A-02 | Implementation | Update the lookup flow to use the appropriate API integration. | High |
| A-03 | Error handling | Define behaviour for empty results and unsuccessful requests. | Medium |
| A-04 | Testing | Prepare checks for successful, empty, and failed responses. | High |
| A-05 | Verification | Review test outcomes and document outstanding issues. | High |


### How to use this artefact

- **Collect:** Identify relevant learning and experiences from the placement.
- **Select:** Include representative work that demonstrates development and problem-solving skills.
- **Reflect:** Explain what the experience taught me about planning, implementation, and quality.
- **Connect:** Show how backlog refinement supports user stories, task breakdown, sprint planning, and verification.

## 6. Reflection

My industry placement has helped me understand that a product backlog includes more than new features. It can also contain defect corrections, API integration work, maintainability improvements, automated testing, and operational workflow enhancements.

For example, work involving points-account retrieval showed me the importance of checking the available API contract before deciding how data should be retrieved. Similarly, automated testing and staging verification demonstrated that product quality depends not only on implementing functionality but also on checking its behaviour and reducing the risk of regressions.

I have also learned that backlog items need to be sufficiently clear before implementation begins. Understanding expected behaviour, dependencies, and acceptance criteria helps developers break work into manageable tasks and make better implementation decisions.

Going forward, I want to improve how I evaluate backlog items by considering business value, technical risk, dependencies, and testability before implementation begins. I also want to make acceptance criteria more specific so that successful completion can be evaluated more consistently.

## 7. Evidence

A prioritisation table based on the backlog items

<img src="{{ '/assets/img/product_backlog_prioritisation_table.png' | relative_url }}" alt="Product Backlog Prioritisation Table">

---

[← Back to portfolio]({{ '/' | relative_url }})