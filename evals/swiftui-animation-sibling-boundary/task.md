# SwiftUI Animation Boundary Routing

## Problem/Feature Description

A SwiftUI dashboard cleanup includes:

- Broad `.animation(.default)` modifiers across whole container views.
- A numeric score label that should animate in place.
- A shared-element card-to-detail transition from a grid.
- A custom adaptive grid layout.
- A deep-link `NavigationStack` path model.
- A request to profile the whole screen for GPU and layout cost.

Explain what the SwiftUI animation skill should own and what should be routed to sibling skills. Include only minimal examples for the animation-owned pieces.

## Output Specification

Create a file named `swiftui-animation-boundary-routing.md` containing:

- Animation work owned by the SwiftUI animation skill.
- Minimal code examples for scoped animation and numeric content transition.
- Sibling-skill routing for navigation, layout, and broader profiling work.
- A short list of boundaries to avoid over-expanding the animation skill.
