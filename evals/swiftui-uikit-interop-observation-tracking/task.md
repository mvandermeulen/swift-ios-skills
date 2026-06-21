# UIKit Observation Tracking Migration

## Problem/Feature Description

A mixed UIKit/SwiftUI app has a `DashboardViewController` that reads an
`@Observable AppState`. It currently starts a `Task` loop, calls
`withObservationTracking`, and then uses `Task.sleep(for: .zero)` to keep
labels refreshed.

Rewrite the approach for an iOS 26-first app. Include the compatibility story
for iOS 18 and for older iOS 15-16 code that still uses `ObservableObject`.

## Output Specification

Create `swiftui-uikit-interop-observation-tracking.md` with:

- The replacement for the polling loop.
- The UIKit methods or handlers that should read observed state.
- The iOS 18 `Info.plist` requirement and whether it applies on iOS 26+.
- The fallback path for iOS 15-16 or existing `ObservableObject` models.
