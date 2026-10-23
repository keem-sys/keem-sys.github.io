---
title: Agile Team Charter
permalink: /agile-team-charter/
---

[← Back to portfolio]({{ '/' | relative_url }})

# Agile Team Charter - Industry Placement

## 1. Project and team context

**Organisation:** Achievements Awards Group (AAG)  
**Student role:** Software Engineering Intern  
**Project scope represented in this portfolio:** Supporting existing business applications and services through frontend development, API integration, database-related work, AWS cloud services, bug fixes, automated testing, code reviews, and deployment or staging verification.

## 2. Shared purpose

Deliver reliable, maintainable improvements to business applications while protecting existing functionality, following the team's development workflow, and communicating progress or blockers early.  

## 3. Working principles

- **Understand before changing:** inspect the existing code, API contracts, data flow, and expected behavior before implementing a change.
- **Communicate progress:** provide concise updates in stand-ups or the team's agreed communication channel.
- **Raise blockers early:** report missing access, unclear requirements, failing dependencies, or environment problems rather than silently losing time.
- **Keep changes focused:** make changes that address the ticket and avoid unrelated refactoring.
- **Use evidence:** validate work with tests, API documentation, database results, and staging checks where appropriate.
- **Review collaboratively:** seek feedback through code review and respond to review comments.
- **Protect data:** do not expose credentials, customer data, client information, or production details in screenshots or public repositories.
- **Own the outcome:** follow work through implementation, testing, review, and verification rather than considering coding alone to be completion.

## 4. Roles and responsibilities

| Role                                    | Responsibility reflected in the placement                                                                                |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Product/business stakeholder            | Clarifies business rules and expected user behaviour.                                                                    |
| Developer / mentor                      | Provides technical guidance, reviews implementation, and helps resolve complex issues.                                   |
| Software Engineering Intern             | Investigates assigned work, implements changes, tests them, communicates status and blockers, and incorporates feedback. |
| Reviewer / team lead                    | Reviews code and helps ensure changes meet team standards before integration.                                            |
| QA / staging verifier, where applicable | Helps verify expected behaviour in the appropriate environment.                                                          |


## 5. Communication and coordination

- **Daily stand-up meetings:** Our team holds a daily stand-up meeting every morning at **09:15**. During these meetings, team members share what they worked on previously, what they are currently working on, and any blockers or challenges that may affect their progress. These meetings help the team stay informed, coordinate activities, and identify issues that require assistance.
    
- **Jira for task management:** We use Jira to create, assign, track, and update development tickets. Tickets are named according to the relevant application or service and the change being implemented, using prefixes such as `webapp-` or `webservices-`. This helps identify which application or service a task relates to and makes work easier to track.
    
- **Bitbucket for source control:** We use Bitbucket to store and manage our source code, track changes through Git, and collaborate on code reviews and pull requests. It provides a central location for managing code contributions and reviewing changes before they are integrated.
    
- **Microsoft Teams for team communication:** Our team has a dedicated Microsoft Teams group where members communicate important updates about ongoing development work. These updates include code being pushed, code reviews, deployment progress, and other project-related announcements. This keeps the team informed about changes and activities that may affect their work.
    
- **Clarifying requirements and blockers:** When acceptance criteria, API behaviour, database dependencies, or implementation details are unclear, I ask the relevant team member or mentor for clarification. This helps me understand the requirements before proceeding and reduces the risk of implementing an incorrect solution.
    
- **Recording progress and decisions:** I use Jira to track the progress of assigned tasks and refer to relevant technical documentation, API specifications, and code review feedback when making implementation decisions. This helps maintain traceability between the original requirement, the implementation, and the verification of the completed work.

- **Sprint coordination:** In addition to daily stand-ups, we use sprint planning meetings to agree on upcoming work, sprint demos to showcase completed work, and retrospectives to identify opportunities for improvement. Jira tickets and their story-point estimates help us organise and discuss the work planned for each two-week sprint.


## 6. Sprint Planning and Agile Ceremonies

Our team works in two-week sprints. Each sprint begins with a sprint planning meeting, during which the team discusses the work to be undertaken during the upcoming sprint. The team reviews the Jira tickets, discusses the requirements and expected outcomes, and agrees on the work to be prioritised.

### Sprint planning and story-point estimation

During sprint planning, story points are assigned to the Jira tickets to estimate the relative effort and complexity of the work. Our team uses a Fibonacci-like sequence, including values such as 1, 3, and 8. This helps the team discuss the relative size of tasks and make more informed decisions about the work planned for the sprint.

### Sprint demo

At the end of the two-week sprint, the team holds a sprint demo meeting to showcase the functionality, improvements, or other work completed during the sprint. This allows the team to demonstrate progress and discuss the outcomes of the work undertaken.

### Sprint retrospective

The team also conducts a retrospective at the end of the sprint. This provides an opportunity to reflect on how the sprint went, identify what worked well, discuss challenges, and consider improvements for the next sprint.

Together with our daily stand-ups, these ceremonies help the team plan work, communicate progress, demonstrate completed work, and continuously improve its development process.

## 7. Definition of ready

Before starting a task, aim to understand:
- the user/business problem;
- expected behaviour and acceptance criteria;
- affected application/API/data components;
- dependencies and required access;
- how the change can be tested.


## 8. Definition of done 

A task is considered complete when the applicable requirements have been met:

- The implementation addresses the agreed requirement and acceptance criteria.
- Relevant automated tests and/or manual checks have been performed.
- Relevant errors, edge cases, loading states, and empty states have been considered.
- Code review feedback has been addressed.
- Changes have been committed and submitted through the team's approved workflow.
- Required staging or environment verification has been completed.
- The Jira ticket has been updated to accurately reflect the work completed, outstanding issues, and verification results.

## 9. Handling disagreements and blockers

1. Reproduce or describe the issue clearly.
2. Gather relevant evidence without exposing sensitive data.
3. Check the ticket, API specification, logs, and existing implementation.
4. Ask the relevant teammate or mentor a focused question.
5. Record the agreed decision in the approved place.
6. Re-test the solution and communicate the outcome.

## 10. Reflection

Working in an existing enterprise codebase has taught me that software development involves more than implementing a feature. Even a relatively small change can depend on API contracts, database data, application architecture, and existing business rules. Understanding these dependencies before writing code helps prevent errors and makes the solution more maintainable.

Our daily stand-up meetings at 09:15 have helped me understand the importance of communicating progress, identifying blockers, and asking for assistance when necessary. For example, while working on a password-reset feature, I connected the frontend to the existing backend functionality. During the review process, I received feedback to move the API calls into the appropriate models and stores rather than handling them directly in the UI components. This required me to revisit my implementation and align it more closely with the application's existing architecture.

Sprint coordination: In addition to daily stand-ups, we use sprint planning meetings to agree on upcoming work, sprint demos to showcase completed work, and retrospectives to identify opportunities for improvement. Jira tickets and their story-point estimates help us organise and discuss the work planned for each two-week sprint.

This experience taught me that getting a feature to work is not the only measure of a good implementation. The code should also follow established design patterns and remain maintainable. It also showed me the value of code reviews as a learning opportunity rather than simply a step towards completing a ticket.

Going forward, I want to improve by understanding the existing architecture before implementation, considering code organisation from the beginning, and communicating uncertainties earlier. I also want to provide more specific stand-up updates that explain what I have completed, what I intend to do next, and whether anything is preventing progress.

## 11. Evidence


<img src="{{ '/assets/img/jira-board.png' | relative_url }}" alt="Jira board (redacted, no company data)">

A Jira board being shown, for company policy reasons I cannot share a true board

<img src="{{ '/assets/img/team-standup.png' | relative_url }}" alt="Microsoft Teams calendar marker for the daily stand-up" width="243">
A teams meeting calendar marker for our daily standup meetings

<img src="{{ '/assets/img/sprint-workflow.png' | relative_url }}" alt="Two-week sprint workflow: planning, daily stand-up, review, retrospective">

The diagram above illustrates the sprint planning, daily stand-ups, sprint demo, and retrospective cycle used by the team.

---

[← Back to portfolio]({{ '/' | relative_url }})
