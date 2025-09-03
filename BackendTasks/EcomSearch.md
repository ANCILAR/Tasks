# E-commerce Search + Cart API — Backend Task

## Summary

Build a backend API for an e-commerce platform that supports **product filtering, sorting, and cart management**. The task involves dynamic query handling and aggregation of cart totals.

## Data Structure

* Products: `{ id, name, category, price, rating, inStock }`
* Cart: List of products added by a user with total cost calculation.

## Goals

* Demonstrate API design, filtering, sorting, and cart aggregation.
* Clean, modular backend with clear routes, middleware, and services.

## Core Requirements

* **GET /products** → Supports filters and sorting:

  * Filters: `category`, `maxPrice`, `minRating`, `inStock`
  * Sorting: `priceAsc`, `priceDesc`, `ratingDesc`
* **POST /cart/add/\:productId** → Adds a product to user’s cart.
* **GET /cart** → Returns cart items + total cost.
* Basic error handling and validation.

## Stretch (optional)

* Pagination for products.
* Remove item from cart.
* Persist cart in database (PostgreSQL/MongoDB).
* Authentication (mock or JWT).

## Candidate Skills Evaluation

1. **API Design** — RESTful routes with clean query parsing.
2. **Filtering & Sorting Logic** — Dynamic handling of multiple filters and sorting keys.
3. **Aggregation** — Correct total cost calculation for cart.
4. **Reusability** — Modular services, reusable utilities.
5. **Error Handling & Validation** — Consistent response structure.

## Submission

* Provide a GitHub repo with README and notes on decisions.
* Include setup and run instructions.

## Evaluation (brief)

* Functionality (filtering, sorting, cart), code quality/types, architecture, reusability, error handling, docs/tests.

## Rating: ⭐⭐⭐⭐