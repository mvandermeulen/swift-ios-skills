# SwiftUI Patterns Migration Accuracy Review

## Problem/Feature Description

A draft iOS 26 SwiftUI migration note says:

- Always mark every `@Observable` type `@MainActor`.
- `Color(uiColor:)` is deprecated and replaced by shader libraries.
- SwiftUI `.copyable`, `.cuttable`, and command-based `.pasteDestination` are iOS 16 APIs.
- `matchedTransitionSource` and `navigationTransition(.zoom)` are iOS 26 only.
- `PreviewProvider`, `EditButton`, and `.onDelete` are deprecated and should always be removed.

Review and correct the guidance.

## Output Specification

Create a file named `swiftui-patterns-migration-accuracy.md` containing:

- A bullet-by-bullet correction.
- Correct availability and deprecation wording.
- A short “modern default” recommendation where an API is still valid but no longer preferred for new code.
