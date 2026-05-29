# SwiftUI Gesture Composition Precedence

## Problem/Feature Description

Review this SwiftUI interaction plan:

- A parent `VStack` attaches `.gesture(TapGesture())`.
- A child image attaches `.onTapGesture`.
- The author says the parent always swallows the child tap, so they want to
  replace every gesture in the feature with `highPriorityGesture`.

Explain the correct precedence model, when to use `.gesture`,
`.simultaneousGesture`, `.highPriorityGesture`, and how `GestureMask` changes
subview participation.

## Output Specification

Create a file named `swiftui-gestures-composition-precedence.md` containing:

- A correction of the parent/child precedence misconception.
- Short Swift snippets for default, simultaneous, and high-priority handling.
- Accurate `GestureMask` guidance for `.gesture`, `.subviews`, `.all`, and
  `.none`.
- A short boundary note for when gesture guidance should hand off to layout,
  navigation, or architecture skills.

Do not create an Xcode project. Keep the answer as implementation guidance and
snippets only.
