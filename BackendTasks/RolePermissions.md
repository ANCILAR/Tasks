# Role & Permission Based Task Manager — Backend Task

## Summary

Build a backend service that implements **Role-Based Access Control (RBAC)** and **permission-based checks** for a task management system. The system should expose APIs to create, update, and retrieve tasks with access restricted by user roles and permissions.

## Roles & Permissions

* Roles: **Admin**, **Manager**, **User**
* Permissions example: `task.create`, `task.update`
* Task schema: `{ id, title, assignedTo, status }`

## Goals

* Demonstrate API design, RBAC logic, middleware, and permission-based filtering.
* Clean, modular code with reusable utilities.

## Core Requirements

* **POST /tasks** → Requires `task.create`.
* **PUT /tasks/\:id** → Requires `task.update`. Only admins can reassign tasks.
* **GET /tasks** → Data filtering:

  * User: sees only their tasks.
  * Manager: sees their team’s tasks.
  * Admin: sees all tasks.
* Middleware: `checkPermission(permission)` → reusable for endpoints.
* Role and permissions to be checked dynamically (mock data or in-memory store acceptable).

## Stretch (optional)

* JWT-based authentication for user roles and permissions.
* Persistent storage (PostgreSQL/MongoDB) instead of in-memory data.
* API for role and permission management.

## Candidate Skills Evaluation

1. **Error Handling & Validation** — Clean responses and validation of inputs.
2. **Architecture** — Clear structure: routes, controllers, middleware, services.
3. **RBAC Logic** — Proper permission checks and role-based data filtering.
4. **Reusability** — Modular middleware, utilities, and services.

## Submission

* Provide a GitHub repo with README and brief notes on decisions.
* Include setup and run instructions.

## Evaluation (brief)

* Functionality (RBAC + permission checks), code quality/types, architecture, reusability, error handling, docs/tests.
## Rating: ⭐⭐⭐⭐⭐