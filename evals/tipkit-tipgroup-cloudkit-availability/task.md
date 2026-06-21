# TipKit Availability and Sync Review

## Problem/Feature Description

An iOS app still supports iOS 17. The product team wants a three-step TipKit
coach-mark sequence that syncs dismissed tips across devices. A draft plan uses
`TipGroup(.ordered)`, `.cloudKitContainer(.automatic)`,
`MaxDisplayDuration(300)`, and says all of this is fine because TipKit is
iOS 17+.

Review the availability and setup risks. Give the team corrected guidance for
iOS 17 support and for an iOS 18+ implementation path.

## Output Specification

Create a file named `tipkit-availability-review.md` containing:

- Which parts of the plan are core iOS 17 TipKit and which are iOS 18+ APIs.
- The iOS 17 fallback options or availability-gating strategy.
- The difference between plain `TipGroup` default priority and `.ordered`.
- CloudKit capability, notification, and container setup risks.
- Correct semantics for `MaxDisplayDuration(300)`.
