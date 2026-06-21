# WeatherKit Dashboard Review

## Problem/Feature Description

An iOS team is building a WeatherKit dashboard that shows the user's current temperature and active weather alert summaries. Their current plan fetches every dataset with `weather(for:)` whenever the SwiftUI view appears, caches responses for exactly 10 minutes, string-interpolates `current.temperature`, prints `alert.region` directly, skips alert detail links, treats `WeatherAvailability` as a broad support matrix for all datasets, and moves Apple Weather attribution to a settings screen.

## Output Specification

Create `weatherkit-dashboard-review.md` with a concise review of what should change before this plan ships. Include corrected WeatherKit query, lifecycle, caching, alert, availability, attribution, temperature formatting, and setup guidance. Code snippets are allowed when they clarify the recommendation.
