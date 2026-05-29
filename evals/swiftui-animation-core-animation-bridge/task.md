# Core Animation Bridge Review

## Problem/Feature Description

An iOS team proposes this SwiftUI/Core Animation bridge guidance:

- Drop to Core Animation for any custom cubic Bezier timing curve because SwiftUI cannot express those curves.
- Use `CADisplayLink.preferredFrameRateRange` to force ProMotion animations to 120 fps.
- In a `UIViewRepresentable`, set `spring.delegate = uiView.next as? CAAnimationDelegate` to notify SwiftUI when a `CASpringAnimation` finishes.

Review the plan and provide corrected modern guidance.

## Output Specification

Create a file named `swiftui-core-animation-bridge-review.md` containing:

- When SwiftUI timing APIs are enough.
- When Core Animation bridging is still appropriate.
- Correct ProMotion/CADisplayLink guidance.
- A corrected `CAAnimationDelegate` Coordinator pattern.
- A short risk list for the original plan.
