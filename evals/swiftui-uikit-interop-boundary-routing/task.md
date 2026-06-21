# SwiftUI/UIKit Interop Boundary Routing

## Problem/Feature Description

A SwiftUI screen needs:

- A PDF viewer.
- A rich text editor.
- A web help center.
- A legacy UIKit share, mail, and message flow.
- A collection view cell that hosts SwiftUI content with swipe actions.

Identify which work belongs in `swiftui-uikit-interop` and which work belongs
in sibling skills. Keep the answer at the boundary-routing and interop-guidance
level rather than turning it into a PDFKit, WebKit, or PhotoKit tutorial.

## Output Specification

Create `swiftui-uikit-interop-boundary-routing.md` with:

- The responsibilities owned by `swiftui-uikit-interop`.
- The PDFKit, WebKit, and rich text handoffs.
- The MessageUI and share-sheet wrapper guidance.
- The `UIHostingConfiguration` guidance for hosted cells and swipe actions.
- Boundaries that should not be expanded into unrelated sibling topics.
