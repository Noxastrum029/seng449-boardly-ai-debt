# Boardly – Specification (v0, draft)

Single specification given to both models (Claude and GPT) in Cursor.

## Functional Requirements
- FR1 User sign-up
- FR2 Login with JWT
- FR3 Create / update / delete projects
- FR4 Create / update / delete tasks within a project
- FR5 Assign a task to a user
- FR6 Change task status (Todo, In Progress, Done)
- FR7 Filter and search tasks
- FR8 Comment on tasks

## Stack
TypeScript · Node.js/Express · Prisma/PostgreSQL · React

## Acceptance
Behavior is defined by >=60 API-level acceptance tests in `tests/acceptance/`, written by the team independently of the AI assistants.
