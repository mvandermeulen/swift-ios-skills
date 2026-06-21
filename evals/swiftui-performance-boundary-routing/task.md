# SwiftUI Performance Boundary Routing

## Problem/Feature Description

A team asks for one review covering a janky SwiftUI screen, a custom transition
whose curve feels wrong, production hang telemetry in MetricKit, and a
NavigationStack deep-link bug. The screen also uses a large scrollable feed and
some expensive row formatting.

Write guidance that says what the `swiftui-performance` skill should handle
directly and what should move to adjacent skills.

## Output Specification

Create a file named `swiftui-performance-boundaries.md` containing:

- The runtime performance items this skill should own.
- The sibling skill handoffs for animation, navigation, MetricKit, and layout or
  architecture work.
- A compact sequencing recommendation for the performance portion.

Do not provide full implementations for the sibling domains.
