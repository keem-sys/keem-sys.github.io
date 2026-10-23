---
title: Product Backlog
permalink: /product-backlog/
---

[← Back to portfolio]({{ '/' | relative_url }})

# Product Backlog – Industry Placement

## 1. Purpose and scope

This product backlog represents software development work I encountered during my industry placement as a Software Engineering Intern in an enterprise software development environment.

The backlog covers improvements to existing business applications and services, including frontend functionality, API integration, data handling, automated testing, operational workflows, and verification in staging environments.

## 2. Product backlog items

| ID    | Backlog item                                                     | User/business value                                                                                            | Portfolio priority |
| ----- | ---------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------ |
| PB-01 | Improve card-status display and filtering                        | Helps users understand whether a card is active, cancelled, or expired.                                        | High               |
| PB-02 | Retrieve points accounts using the appropriate API endpoint      | Improves the accuracy and maintainability of person-and-campaign account lookups.                              | High               |
| PB-03 | Integrate the password-reset interface with the existing backend | Supports account recovery while keeping API communication within the appropriate application layers.           | High               |
| PB-04 | Improve redemption retrieval and pagination                      | Helps authorised users retrieve and navigate redemption records consistently.                                  | High               |
| PB-05 | Protect sensitive voucher identifiers in the interface           | Reduces unnecessary exposure of sensitive identifiers in relevant views.                                       | High               |
| PB-06 | Replace hardcoded catalogue rules with data-driven logic         | Reduces fragile assumptions and improves maintainability when catalogue data changes.                          | Medium             |
| PB-07 | Correct catalogue and service integration issues                 | Improves reliability by aligning application behaviour with current API contracts and expected business rules. | High               |
| PB-08 | Improve loading, empty, and error states                         | Helps users understand what is happening when data is unavailable or a request fails.                          | Medium             |
| PB-09 | Maintain and repair automated tests                              | Helps detect regressions and increases confidence in code changes.                                             | High               |
| PB-10 | Improve operational document generation and printing             | Supports reliable document generation, display, and printing for operational workflows.                        | Medium             |
| PB-11 | Correct form input and endpoint integration behaviour            | Improves input handling and reduces avoidable request failures.                                                | Medium             |
| PB-12 | Verify changes and record test outcomes                          | Helps establish that changes meet requirements and work in the appropriate environment.                        | High               |


## 3. Backlog prioritisation

The suggested priorities consider the potential effect of each item on functional correctness, user experience, maintainability, data protection, and regression risk.

Items involving incorrect data retrieval, account recovery, sensitive identifiers, or core functionality are assigned higher illustrative priorities because defects in these areas could have a significant impact. Testing and verification are also important because they help establish confidence that changes have not introduced regressions.

## 4. Backlog refinement and task breakdown

A backlog item should be understood and refined before it is selected for implementation. Depending on the work involved, this may include:

1. Clarifying the user or business problem.
    
2. Defining the expected behaviour and acceptance criteria.
    
3. Reviewing relevant code, API specifications, and dependencies.
    
4. Breaking the work into smaller development and testing tasks.
    
5. Discussing relative complexity during sprint planning and assigning story points.
    
6. Confirming the expected verification and review requirements.
    

During my placement, I encountered work that required investigating existing application behaviour, checking API documentation, adapting implementations, addressing review feedback, and verifying changes. These experiences showed me why backlog refinement needs to consider more than the coding effort alone.

## 5. Relationship between the product backlog and sprint backlog

The product backlog represents a broader collection of potential improvements, defects, and maintenance work. The sprint backlog represents the work selected for a particular two-week sprint, together with the plan for delivering it.

During sprint planning, the team discusses upcoming work and estimates its relative complexity using story points. Once work is selected, individual tasks can be used to organise implementation, testing, and review. Daily stand-ups help the team communicate progress and blockers, while the sprint demo and retrospective provide opportunities to review outcomes and identify improvements.

The items in this portfolio are not assigned to specific sprints because I have not reproduced the team's actual sprint records.

## 6. Evidence

The following portfolio-safe artefacts support this backlog:

<img src="{{ '/assets/img/jira-board.png' | relative_url }}" alt="Jira board (redacted, no company data)">

A redacted Jira board view. For company policy reasons I cannot share the real board.

## 7. Reflection

My industry placement has helped me understand that a product backlog includes more than new features. It can also contain defect corrections, API integration work, maintainability improvements, automated testing, and operational workflow enhancements.

For example, work involving points-account retrieval showed me the importance of checking the available API contract before deciding how data should be retrieved. Similarly, automated testing and staging verification demonstrated that product quality depends not only on implementing functionality but also on checking its behaviour and reducing the risk of regressions.

I have also learned that backlog items need to be sufficiently clear before implementation. Understanding the expected behaviour, dependencies, and acceptance criteria helps developers break work into manageable tasks and make better implementation decisions.

Going forward, I want to improve how I evaluate backlog items by considering business value, technical risk, dependencies, and testability before implementation begins. I also want to make acceptance criteria more specific so that the team can better understand what successful completion looks like.

---

[← Back to portfolio]({{ '/' | relative_url }})
