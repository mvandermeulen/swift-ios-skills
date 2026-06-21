# SwiftUI Feed Performance Review

## Problem/Feature Description

An iOS 26 SwiftUI feed stutters while scrolling. Each row builds a formatted
subtitle, decodes thumbnail data, filters badges inline, and some sponsored rows
host a UIKit video preview through `UIViewRepresentable`.

The team has not collected a trace yet. They want a concise plan for what to
record and the first code areas to inspect once the trace is available.

## Output Specification

Create a file named `swiftui-feed-performance-review.md` containing:

- The profiling setup to collect reliable evidence.
- The current SwiftUI Instruments lanes or graph views to inspect.
- How to correlate SwiftUI-specific data with Time Profiler or Hangs/Hitches.
- The likely first remediation targets in the row code.
- Any boundaries that keep the recommendation focused on runtime performance.

Do not write a complete replacement feed implementation.
