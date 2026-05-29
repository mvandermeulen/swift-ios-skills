# Event Card Display Review

## Problem/Feature Description

An iOS 16 SwiftUI event card shows the event landing page and the last update time with this code:

```swift
Text(eventURL.formatted())
Text("Updated \(updatedAt.formatted(.relative(presentation: .named)))")
```

Support staff use the displayed landing page to distinguish campaign links and staged event hosts. The localization reviewer also flagged the update label as risky for natural-sounding UI in languages with different grammar than English.

## Output Specification

Create `event-card-format-review.md` that:

- audits the two displayed values,
- provides corrected Swift snippets for the event card,
- notes any platform availability that matters for an iOS 16 target,
- and keeps the recommendation focused on formatting behavior.
