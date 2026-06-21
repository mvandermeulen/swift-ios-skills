# SwiftUI NavigationStack Route Review

## Problem/Feature Description

A team is planning navigation for an iOS 26 SwiftUI app with Home, Search, and Profile tabs. The draft says:

- Use one global `NavigationPath` because it is the type-safe choice.
- Push complete `Item` models into the path from every tab.
- Reset the shared path whenever the user switches tabs.

Review and correct the plan.

## Output Specification

Create a file named `swiftui-navigation-route-review.md` containing:

- The recommended route/path model for app-owned push destinations.
- How each tab should own or receive navigation state.
- What data should be stored in navigation routes.
- A minimal Swift example.
