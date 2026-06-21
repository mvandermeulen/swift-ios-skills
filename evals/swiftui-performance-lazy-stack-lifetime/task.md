# Lazy Stack Runtime Review

## Problem/Feature Description

A custom SwiftUI timeline uses `ScrollView` plus `LazyVStack`. Users report that
draft text typed into offscreen rows sometimes disappears after scrolling away
and back. Programmatic scroll-to-id sometimes lands slightly wrong while rows
load. The row builder also contains this pattern:

```swift
ForEach(items) { item in
    if item.isVisible {
        TimelineRow(item: item)
    }
}
```

Some rows use geometry changes to update shared timeline state.

## Output Specification

Create a file named `lazy-stack-runtime-review.md` containing:

- The likely lazy stack lifetime and state-retention issue.
- The `ForEach` row-shape and identity risks.
- The scroll offset/content-size caveat.
- The geometry feedback risk and safer alternatives.
- A brief checklist of corrections.

Do not rewrite the screen.
