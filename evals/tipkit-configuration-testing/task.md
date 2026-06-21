# TipKit Setup Review

## Problem/Feature Description

An iOS app team is adding TipKit for first-run feature discovery. Their draft
plan calls `Tips.configure()` from `ContentView.task`, has UI tests call
`Tips.resetDatastore()` after the app launches, ships
`Tips.showAllTipsForTesting()` behind a custom runtime flag, and sets every tip
to show immediately so onboarding is visible on first launch.

Review the plan and provide corrected Swift-oriented guidance. Keep the answer
focused on TipKit setup, testing, and display policy; do not design a full
onboarding product flow.

## Output Specification

Create a file named `tipkit-setup-review.md` containing:

- Where and when `Tips.configure(_:)` should run.
- How test resets and forced-tip visibility should be applied.
- Why test-only overrides must not ship as production behavior.
- A concise UI-test launch-argument example.
- Guidance for production display frequency, rules, and invalidation.
