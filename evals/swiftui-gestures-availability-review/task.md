# SwiftUI Gesture API Availability Review

## Problem/Feature Description

Audit this SwiftUI gesture guidance for an iOS 26 app:

- Use `MagnificationGesture` and `RotationGesture` because they are still the
  newest types.
- `DragGesture.Value.velocity` is only safe on iOS 17 and later.
- `UIGestureRecognizerRepresentable` can be used on any iOS 16 SwiftUI screen.

Give corrected modern guidance with availability notes and source links.

## Output Specification

Create a file named `swiftui-gestures-availability-review.md` containing:

- Correct modern replacements for pinch/magnification and rotation gestures.
- Correct availability guidance for `DragGesture.Value.velocity`.
- Correct availability and scope for `UIGestureRecognizerRepresentable`.
- Sosumi or official Apple documentation URLs for the API availability claims.

Do not create an Xcode project. Keep the answer as implementation guidance and
snippets only.
