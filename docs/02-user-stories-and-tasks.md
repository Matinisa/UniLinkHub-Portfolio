# 2\. User Stories and Tasks — UniLink Hub

## 2.1 Requirements background

The team identified a need for students to discover products and services offered by student entrepreneurs more easily. Requirements were gathered through discussions, interviews and group-chat messages about difficulties finding student-owned offerings.

The stories below are reconstructed from the functionality described for the project:

## 2.2 User stories

| ID | User story | Priority | Related tasks / acceptance evidence |
| --- | --- | --- | --- |
| US-01 | As a student, I want to register for an account so that I can use the marketplace. | High | Create registration UI and API; validate submitted details; store account data; test successful and unsuccessful registration. Attach authentic registration/API evidence. |
| US-02 | As a student, I want to verify my email so that the system can confirm my email address. | High | Implement the email-verification flow; test the flow with valid and invalid/expired tokens where supported. Confirm the final behaviour from the running project. |
| US-03 | As a student browsing the marketplace, I want to search or filter listings so that I can find relevant products or services. | High | Build search/filter controls; connect them to available listing data; test representative searches and filters. |
| US-04 | As a student, I want to view a listing's details, price, location and images so that I can decide whether it meets my needs. | High | Create listing detail view; display available business/product/service information; test with real project data. |
| US-05 | As a student entrepreneur, I want to create a business profile so that other students can discover my business. | High | Provide the entrepreneur entry point; collect business details; validate and save the profile; test profile creation. |
| US-06 | As a student entrepreneur, I want to add products or services with prices, images and locations so that students understand what I offer. | High | Build listing form; handle listing fields and images where implemented; save and display listings; test create/edit behaviour. Confirm any incomplete image handling. |
| US-07 | As an entrepreneur, I want to edit or delete my own listings so that I can keep information up to date. | Medium | Add owner-authorised update/delete operations; check that users cannot manage another entrepreneur's listings; test both allowed and denied cases. |
| US-08 | As a student, I want to contact or express interest in a provider so that I can ask about a product or service. | High | Display provider contact information; provide the messaging/interest interaction where implemented; test the interaction. Confirm whether messaging was fully completed. |
| US-09 | As an entrepreneur, I want to receive a notification when a student expresses interest so that I can respond. | Medium | Record interest; notify the entrepreneur; allow the notification to open the relevant panel/details; test the notification path. |
| US-10 | As an administrator, I want to review or verify registrations and business providers so that marketplace participation can be checked. | Medium | Provide admin review controls and backend checks; test the relevant admin permissions and review states. Confirm exact implemented scope. |
| US-11 | As a student, I want to edit my profile so that my account information remains current. | Medium | Provide profile editing; validate updates; persist changes; test the updated profile. |
| US-12 | As a user, I want to choose a light or dark appearance so that the interface is comfortable to use. | Low / improvement | Confirm whether a theme preference feature exists. If not completed, keep this as a future improvement rather than claiming it is implemented. |

## 2.3 My tasks: backend and database

My individual responsibility was mainly backend and database connection work. The following task list reflects the work I described:

-   Implement backend functionality using Java and Spring Boot.
-   Work on Spring Security and registration/security behaviour.
-   Create or connect REST API endpoints to support the frontend.
-   Test registration and API behaviour with Postman.
-   Test database connectivity using MySQL.
-   Test password encryption/hashing behaviour.
-   Troubleshoot security/API responses and backend integration issues.
-   Support integration between the backend and frontend.

Use GitHub commit history, relevant code files and safe Postman screenshots to demonstrate which tasks I personally completed. Do not include credentials, real user passwords, tokens or other secrets.

## 2.4 Task decomposition example

**Story US-01: Register an account**

1.  Identify the required registration fields.
2.  Create or connect the registration endpoint.
3.  Validate the incoming request.
4.  Apply the intended password-protection mechanism.
5.  Save the account through the persistence layer.
6.  Test successful and unsuccessful requests in Postman.
7.  Record the observed result and fix any issues found.

This is a useful breakdown of the work, but only mark individual tasks as completed when supported by the code, test results or project records.

## 2.5 Evidence to attach

### Evidence 2.1: User Story Evidence

![UniLink Hub team meeting](http://localhost:62964/images/Trello-User-Story-1.png) ![UniLink Hub team meeting](http://localhost:62964/images/Trello-User-Story-2.png)

**Figure 1: Conducted User Story**

**Purpose:** The screen shorts above serves as evidence for the conducted user stories behind the production of the system

**Reflection:** User stories assisted us a lot on mapping excactly what the user expect to see on the system, and the type of problem we trying to solve. The usage of user story is like being placed inside the user's shoes, making it faccilitative to easly satisfy user,s needs

### Evidence 2.2: Git Commits

![UniLink Hub team meeting](../images/G-Commits-1.png)

**Figure 2: GitHub Repo Commits**

**Purpose:** The screenshots above serves as evidence for the conducted user stories behind the production of the system

**Reflection:** User stories assisted us a lot on mapping excactly what the user expect to see on the system, and the type of problem we trying to solve. The usage of user story is like being placed inside the user's shoes, making it faccilitative to easly satisfy user,s needs

### Evidence 2.3: API test Evidence

![UniLink Hub team meeting](http://localhost:62964/images/Api-Test-1.png) 
![UniLink Hub team meeting](http://localhost:62964/images/Api-Test-2.png)

**Figure 3: API end-point test**

**Purpose:** These are the API end-points used 
to test the back-end of the system, to check is the severside works correctly,
and testing some CRUD methods os the system.

**Reflection:** Using postman for API testing has made it easy for us and sped up the process, 
rather using the old traditional way

## 2.6 Reflection

Writing requirements as user stories helps connect development work to a real user need rather than treating a feature as code in isolation. Breaking a story into smaller tasks also makes it easier to estimate what must be built and tested. In my backend role, I learned that an endpoint is not complete just because the code compiles: the request, security rules, database operation and response must work together. I need to improve how consistently I record acceptance criteria and test evidence so that completion can be verified by another team member.
