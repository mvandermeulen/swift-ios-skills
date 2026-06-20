# Floating Tool Palette Guidance

## Problem/Feature Description

A drawing app is replacing a custom blur palette with the iOS 26 design system. The palette
contains three icon controls for Pencil, Eraser, and Lasso. Tapping a disclosure button
reveals two extra tools and animates the palette between compact and expanded states. The
current prototype stacks several translucent wrappers around each icon and uses model
objects directly as animation identifiers.

Give concise SwiftUI implementation guidance for the palette. Keep the answer focused on
the glass treatment and transition behavior, not the drawing model.

## Output Specification

Create a file named `swiftui-liquid-glass-tool-palette.md` containing:

- A short implementation plan.
- A SwiftUI snippet showing the grouped controls and expansion behavior.
- Notes about identifiers, modifier order, and availability.
- A short list of mistakes to avoid.
