# SwiftUI Sheet Dismissal Review

## Problem/Feature Description

A team is writing iOS 26 SwiftUI sheet guidance. The draft says:

- Call `dismissalConfirmationDialog` from every editing sheet to block accidental dismissal.
- Use custom frames to size form-style sheets.
- Drive all modal presentation from Boolean flags.

Review and correct the guidance using current SwiftUI sheet APIs.

## Output Specification

Create a file named `swiftui-sheet-dismissal-review.md` containing:

- Correct dismissal-prevention guidance for iOS/iPadOS editing sheets.
- The macOS-specific dismissal confirmation note, if relevant.
- Modern sheet sizing guidance.
- Recommended state/routing shape for model-backed sheets.
