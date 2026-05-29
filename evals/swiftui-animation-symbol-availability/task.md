# SwiftUI Symbol Animation Review

## Problem/Feature Description

A team is preparing an iOS 26 SwiftUI animation guide. The draft says:

- Use `Image(systemName: "wifi").symbolVariableColor(value: signal)` for variable SF Symbol fill.
- Treat `.wiggle`, `.breathe`, and `.rotate` as iOS 17 symbol effects.
- Use `.symbolEffect(.wiggle.clockwise, value:)` and `.symbolEffect(.breathe, isActive:)` with no availability note.

Review and correct the guidance.

## Output Specification

Create a file named `swiftui-symbol-animation-review.md` containing:

- Correct variable SF Symbol value guidance with a minimal Swift example.
- Correct symbol effect availability guidance.
- A short corrected example for discrete and indefinite symbol effects.
- Any Reduce Motion caveat that applies to repeating or active symbol effects.
