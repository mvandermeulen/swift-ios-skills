# SwiftUI Gesture Boundary and Accessibility Review

## Problem/Feature Description

A custom card grid uses:

- `onTapGesture` for every delete action.
- Drag gestures for reordering.
- A custom swipe recognizer.
- A request to clean up navigation routing and grid layout in the same patch.

Which parts belong in the SwiftUI gestures skill, what accessibility fixes
should be made for gesture-only actions, and what should be handed to sibling
skills?

## Output Specification

Create a file named `swiftui-gestures-boundary-accessibility.md` containing:

- The gesture-specific work that belongs in `swiftui-gestures`.
- Corrections for plain single-tap actions that should be `Button`s.
- Accessible alternatives for drag, swipe, or other gesture-only interactions.
- Handoffs to sibling skills for layout, navigation, and broad state
  architecture.

Do not create an Xcode project. Keep the answer as implementation guidance and
snippets only.
