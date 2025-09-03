# Case-Insensitive Login + Rate Limiting — Backend Task

## Summary

Build a backend API to handle user signup and login with case-insensitive checks and rate limiting on login attempts.

## Goals

* Implement case-insensitive username and email uniqueness.
* Securely store passwords using hashing (e.g., SHA256/base64).
* Enforce login rate limiting to prevent brute-force attacks.

## Core Requirements

* **POST /signup** → Create a new user with unique username & email (case-insensitive).
* **POST /login** → Authenticate user with case-insensitive username/email.
* Rate limit: max **5 login attempts per user within 10 minutes**.

  * If exceeded → return **429 Too Many Requests**.
* Store users in-memory (no DB required).

## Stretch (optional)

* Add JWT-based authentication after successful login.
* Password reset or email normalization utility.
* Configurable rate limit window.


## Rating: ⭐⭐