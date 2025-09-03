# Users Table — Frontend Task

## Summary

Fetch user data from the provided API and display it in a table. Implement client-side sorting for every displayed column. Keep the implementation clean, reusable, and delivery-ready.

api - https://jsonplaceholder.typicode.com/users

## Goals

* Demonstrate data fetching, table UI, sorting, and basic UX.
* Prefer TypeScript and clear component structure.

## Core Requirements

* Fetch users from the provided API.
* Display results in a table (columns: name, email, phone, and any other fields provided).
* Implement sorting for every column (ascending/descending toggle).
* Handle loading and error states with user-friendly messages.
* Make sorting client-side and stable.

## Stretch (optional)

* Implement search/filter across columns (extra edge).
* Add pagination or virtualized rows for large lists.
* Column-specific filters (e.g., by domain or phone prefix).

## Candidate Skills Evaluation

1. **TypeScript vs JavaScript** — TypeScript preferred; JavaScript acceptable. Look for types for API responses and components.
2. **Styling** — Tailwind preferred; keep it responsive and accessible.
3. **State Management** — Use **Redux** preferred; Zustand acceptable. Keep fetch/state separation clear (hooks like `useUsers`).
4. **Reusability** — Reusable table and sorting logic (hooks/util), small composable components.

## Submission

* Provide a GitHub repo with README and brief notes on decisions.
* Include run instructions and any shortcuts or missing pieces.

## Evaluation (brief)

* Functionality (fetch + sort \[+search]), code quality/types, state architecture, reusability, styling/UX, docs/tests.
## Rating: ⭐⭐⭐⭐