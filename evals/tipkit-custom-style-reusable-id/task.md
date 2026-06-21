# TipKit Custom UI Review

## Problem/Feature Description

An app team is building a custom TipKit UI. Their reusable `NewItemTip` does
not override `id`, a custom `TipViewStyle` reads title/message/actions directly
from a captured concrete `NewItemTip` instance, the style renders
`Button(action: action.handler) { action.label }`, event donations persist a
large app model object, and the user action never invalidates the tip.

Review the plan and give corrected Swift-oriented guidance. Keep the answer
focused on TipKit custom UI behavior and persistence.

## Output Specification

Create a file named `tipkit-custom-ui-review.md` containing:

- How reusable tips should define stable custom IDs.
- How custom `TipViewStyle` implementations should use configuration values.
- The correct action label and handler invocation shape.
- Guidance for event donation payload size and type constraints.
- Where and why to invalidate the tip after the discovered action.
