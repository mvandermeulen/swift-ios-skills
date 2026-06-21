# SwiftUI External Routing Review

## Problem/Feature Description

A team is reviewing an iOS 26 SwiftUI routing note. The draft says:

- Universal Links should be handled primarily with `onContinueUserActivity` for web-browsing activities.
- AASA updates take 24-48 hours to propagate.
- `Tab(role: .search)` replaces the tab bar with a search field when selected.

Review and correct the note.

## Output Specification

Create a file named `swiftui-external-routing-review.md` containing:

- The SwiftUI hook to use for Universal Links and custom URL schemes.
- Where Handoff or other user activities fit.
- Correct AASA cache/debugging guidance.
- Correct iOS 26 search tab role guidance.
