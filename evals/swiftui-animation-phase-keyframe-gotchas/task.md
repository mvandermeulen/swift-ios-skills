# SwiftUI Phase and Keyframe Animation Review

## Problem/Feature Description

A SwiftUI animation note says:

- `PhaseAnimator(phases, trigger: tapCount)` runs through every phase once each time `tapCount` changes.
- A tap-triggered "like" burst should use trigger-based `PhaseAnimator` for the full sequence.
- Swift 6 code can freely read `@State` and `@Environment` values from nested helper closures inside `keyframeAnimator`.

Review and correct the guidance for modern SwiftUI.

## Output Specification

Create a file named `swiftui-phase-keyframe-review.md` containing:

- Correct trigger-based `PhaseAnimator` semantics.
- A minimal alternative for a full tap-triggered animation timeline.
- Swift 6 guidance for `@Sendable` keyframe closures.
- A short boundary note that keeps layout or navigation architecture out of scope.
