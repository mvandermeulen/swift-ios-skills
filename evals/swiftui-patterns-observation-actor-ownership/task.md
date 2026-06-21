# SwiftUI Observation State Ownership Review

## Problem/Feature Description

A team is designing an iOS 26 SwiftUI profile settings screen. The screen edits a profile name, persists a theme preference, loads remote suggestions asynchronously, and passes editable state into child field views.

They propose:

- Put all state in an `@Observable` `ProfileSettingsStore`.
- Mark every model in the feature `@MainActor`, including plain decoded profile DTOs.
- Store the theme preference with `@AppStorage` inside the observable store.
- Pass the store to child views and use `$store.name` directly.
- Start suggestion loading from `onAppear { Task { ... } }`.

Review and correct the architecture.

## Output Specification

Create a file named `swiftui-patterns-observation-actor-ownership.md` containing:

- A corrected ownership sketch using modern Observation.
- Clear guidance for `@MainActor`, `@State`, `@Bindable`, `@Environment`, and `.task`.
- Correct guidance for the theme preference persistence.
- At least one concise Swift example.
