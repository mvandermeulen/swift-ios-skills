# Sheet Header Liquid Glass Review

## Problem/Feature Description

The options team is updating an iOS 26 SwiftUI sheet header. The header has a centered
title, a trailing Done action, and a leading number that shows how many contracts expire
today. A prototype puts the number in the top toolbar as a rounded translucent capsule.
During review, people keep tapping the number because it visually reacts even though it
does not open anything.

Provide implementation guidance that resolves the ambiguity and keeps the sheet aligned
with the current iOS 26 design system. The team wants a recommendation, not a full app.

## Output Specification

Create a file named `swiftui-liquid-glass-status-affordance.md` containing:

- The recommended treatment for the count.
- Any SwiftUI snippets needed to show the corrected approach.
- Accessibility and verification notes.
- A short explanation of what should remain in the toolbar.
