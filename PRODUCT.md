# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Product Purpose

A minimalist, mobile-friendly gym progress app. Help the user understand workout progress through a simple interface that works well on a phone.

## Users

Open decision: whether this serves the owner as a personal dashboard or other gym-goers who record their own workouts.

## Operating Context

The existing implementation is a single-page web dashboard in `index.html`. It reads workout records and progress summaries from `https://gym-api.senthil.nz`. The calendar currently uses the Pacific/Auckland timezone.

Open decision: how workout records are collected before reaching the API.

## Capabilities and Constraints

Repository evidence establishes these current capabilities; it does not establish that each is a permanent product requirement:

- Active, individual, and combined workout goal progress.
- Current and longest streaks.
- Weekly workout progress and comparison messaging.
- Upcoming milestones and workouts remaining.
- Workout frequency and goal forecasts.
- Calendar history with Pull, Push, Legs, and Cardio categories.
- Calendar navigation and light/dark theme switching.

The current page reads data and has no workout-entry interface. Whether to retain this read-only workflow or add logging is undecided.

The existing frontend uses plain HTML and JavaScript with CDN-loaded Basecoat CSS, Tailwind, D3, and Cal-Heatmap. No backend implementation or build setup is present in this repository.

## Brand Commitments

The user requests a minimalist app and mobile-friendly use. Preserve these commitments in future design decisions.

The current page uses the name “Gym Journey”; a permanent name has not been confirmed.

## Evidence on Hand

- `index.html`: current interface, copy, API integration, and behavior.
- `mock.png`: existing visual reference with 2025 example content; its numbers are illustrative, not verified workout data.

## Product Principles

- Keep understanding gym progress the central task.
- Keep the interface minimal and easy to use on a phone.
- Ground progress summaries in actual workout data.

## Open Decisions

- Primary audience and whether workout logging belongs in this app.
- Durable API, privacy, and accessibility requirements beyond mobile-friendly use.
- Any positioning claim beyond straightforward gym progress tracking.
