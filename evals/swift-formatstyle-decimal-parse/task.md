# Finance Amount Formatting Cleanup

## Problem/Feature Description

The Ledger Pro iOS 17 finance screen still uses a shared formatter helper from an older UIKit module. The source amount is stored as `Decimal`, but a recent patch converted it through `Double` before showing the value and before importing edited CSV amounts such as `$3,500.63`.

Operations reported occasional penny mismatches after a user edits an exported value and imports it again. The team wants a short review and a replacement pattern using current Swift formatting APIs that can be reused from SwiftUI display code and import code.

## Output Specification

Create `amount-formatting-review.md` with:

- a concise diagnosis of the risk in the current approach,
- replacement Swift snippets for display and parsing,
- a note about how finance QA should check locale-sensitive behavior,
- and any ownership boundary that keeps this cleanup scoped.
