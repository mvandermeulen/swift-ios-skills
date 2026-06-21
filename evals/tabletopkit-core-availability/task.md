# TabletopKit Board Game Setup Review

## Problem/Feature Description

The visionOS team is starting a multiplayer tabletop board game with a board, movable pieces, player seats, a die, and a SwiftUI control surface. The first release must support visionOS 2.x where possible, while allowing newer TabletopKit APIs to be adopted when the runtime supports them.

Write an implementation note for the team that covers the app-side game setup, core TabletopKit types, player interaction model, RealityKit rendering boundary, and availability gates for newer APIs. The note should help an engineer avoid accidentally making a visionOS 2.x feature depend on visionOS 26-only TabletopKit APIs.

## Output Specification

Create `tabletopkit-board-setup.md` with Swift-oriented implementation guidance, concise snippets where useful, and a short review checklist. Do not create an Xcode project.
