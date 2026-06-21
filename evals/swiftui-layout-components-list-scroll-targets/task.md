# SwiftUI Settings Layout Review

## Problem/Feature Description

An iOS 26 settings screen is currently built with `List` and many `Section`s.
Product wants a compact jump control that can move directly to any section.
Several rows also expand in place to show longer descriptions, and design wants
to avoid jarring layout jumps without turning this review into animation tuning
guidance.

Write guidance for the team choosing the right SwiftUI container and interaction
pattern. The answer should keep native settings behavior where it fits, but it
should also call out when a custom scroll layout is the better engineering
choice.

## Output Specification

Create a file named `swiftui-settings-layout-review.md` containing:

- The default `List`/`Form` starting point and the conditions that justify
  switching to a custom scroll layout.
- How to distinguish simple edge scroll actions from direct section or item
  jumps, including the custom scroll-target container/API pattern when direct
  jumps justify leaving `List`/`Form`.
- How to treat expanding row descriptions as a layout/container tradeoff,
  without animation implementation advice.
- Any important identity, scrolling, or accessibility constraints.
- Boundaries for what should remain normal `List`/`Form` guidance.

Do not include Swift view/component implementations or animation modifier
examples. Keep API mentions brief and tied to the layout decision.
