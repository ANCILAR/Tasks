# Inventory + Reservation System with Expiry — Backend Task

## Summary

Build a backend API to manage product inventory with a reservation system that expires after a set time. Reservations should auto-expire if not confirmed, returning stock back to inventory.

## Data Structure

* Product: `{ id: string, name: string, stock: number }`
* Reservation: `{ id: string, productId: string, expiresAt: Date, status: "reserved" | "confirmed" }`

## Goals

* Demonstrate temporary state handling, reservation expiry, and stock management.
* Implement cleanup of expired reservations.

## Core Requirements

* **POST /reserve/\:productId** → Decrease stock by 1 and create a reservation (expires in 30s if not confirmed).
* **POST /confirm/\:reservationId** → Confirm a reservation, remove it from pending list.
* Expired reservations should auto-return to stock (timer-based or cleanup job).
* Handle concurrency and prevent over-reserving.

## Stretch (optional)

* GET /products → List products with current stock.
* GET /reservations → View pending/confirmed reservations.
* Configurable expiry duration.
* Persistent storage (database) instead of in-memory.

## Candidate Skills Evaluation

1. **Error Handling & Validation** — Consistent and reliable.
2. **API Design** — Clean RESTful routes with status handling.
3. **Timer & Cleanup Logic** — Proper implementation of expiry and stock rollback.
4. **Concurrency Handling** — Safe stock decrement.
5. **Reusability** — Modular services and utilities.

## Submission

* Provide a GitHub repo with README and notes on decisions.
* Include setup and run instructions.

## Evaluation (brief)

* Functionality (reservation + expiry), code quality/types, concurrency handling, reusability, error handling, docs/tests.
## Rating: ⭐⭐⭐