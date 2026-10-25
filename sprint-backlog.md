---
title: Sprint Backlog
permalink: /sprint-backlog/
---

[← Back to portfolio]({{ '/' | relative_url }})

# Sprint Backlog – Industry Placement

## 1. Purpose and context

This sprint backlog demonstrates how product backlog items can be refined into a focused plan for a two-week development sprint.

It draws on the types of software development work I encountered during my industry placement as a Software Engineering Intern. The examples cover API integration, frontend development, automated testing, code review, and verification.

## 2. Sprint planning approach

Our team works in two-week sprints. At the beginning of each sprint, we hold a sprint planning meeting to discuss the work planned for the upcoming period. Jira tickets are reviewed, and story points are assigned using a Fibonacci-like estimation sequence, including values such as 1, 3, and 8.

The team discusses the intended work and its relative complexity before implementation begins. During the sprint, daily stand-ups provide an opportunity to communicate progress, current priorities, and blockers.

At the end of the sprint, the team holds a demo to showcase completed work and a retrospective to reflect on the process and identify potential improvements.

## 3. Sprint goal

Improve the reliability and maintainability of existing application functionality by aligning frontend behaviour with the appropriate API contracts and verifying changes through testing and code review.

## 4. Sprint work items

| Work item | Planned tasks | Dependencies and risks | Definition of success |
|---|---|---|---|
| Points-account API integration | Confirm the endpoint contract; implement the lookup using the required identifiers; test relevant response cases. | API availability, accurate documentation, and expected response structure. | The application uses the appropriate endpoint and handles expected results correctly. |
| Card-status behaviour | Confirm the status rules; update filtering or display logic; test active, cancelled, expired, and empty-result cases. | Correct API fields and agreed business rules. | Card statuses are displayed and filtered consistently with the requirements. |
| Password-reset integration | Trace the existing frontend-to-backend flow; connect the OTP and reset interactions; test success and failure cases; address review feedback. | Existing backend behaviour and established frontend architecture. | The flow works as intended and follows the application's established code organisation. |
| Automated test maintenance | Investigate failing tests; determine whether the issue is in the tests or implementation; make corrections and rerun the suite. | Test environment and current service behaviour. | Relevant tests pass and the results are recorded accurately. |

## 5. Task tracking and progress

A sprint backlog makes the work needed to achieve the sprint goal visible and manageable. Each selected item can be broken into smaller tasks covering investigation, implementation, testing, review, and verification.

| Task stage | Purpose |
|---|---|
| Investigation | Understand the existing implementation, requirements, and dependencies. |
| Implementation | Make the focused code or configuration changes required by the task. |
| Testing | Validate expected behaviour and relevant failure cases. |
| Code review | Submit the change for review and address feedback. |
| Verification | Confirm the outcome in the appropriate environment and record the result. |

This breakdown helps make the work involved in completing a backlog item clearer and ensures that testing and review are considered alongside implementation.

## 6. Managing blockers and changes

During development, tasks may require additional investigation when API documentation changes, test failures occur, or implementation details are unclear. When this happens, the developer should investigate the issue, consult relevant documentation, and seek clarification where necessary.

Daily stand-ups help communicate these issues so that dependencies and decisions can be addressed. Changes to planned work should also be communicated and managed in accordance with the team's process.

My placement experience has shown me that effective planning needs to account for testing, code review, and dependencies rather than focusing exclusively on implementation.

## 7. Reflection

Working in a two-week sprint environment has helped me understand how planned work is organised into manageable tasks. Sprint planning establishes what the team intends to work on, story-point estimation supports discussions about relative complexity, and daily stand-ups provide opportunities to communicate progress and blockers.

My development experience has also shown me that the steps needed to complete a task can change as I learn more about the existing application. For example, checking an updated API contract can lead to a different implementation approach, while code review feedback can require changes to how API calls are organised in the frontend.

These experiences have reinforced the importance of including investigation, testing, and review in the task breakdown. Going forward, I want to identify dependencies earlier, make acceptance criteria more specific, and communicate risks as soon as they become apparent.

## 8. Evidence

<img src="{{ '/assets/img/sprint-workflow.png' | relative_url }}" alt="Two-week sprint workflow diagram">

The sprint cycle used by the team: sprint planning, daily stand-up, sprint review (demo), retrospective and backlog update.

---

[← Back to portfolio]({{ '/' | relative_url }})