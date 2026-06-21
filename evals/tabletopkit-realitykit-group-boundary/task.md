# TabletopKit Multiplayer Architecture Note

## Problem/Feature Description

The team is planning a spatial tabletop game for visionOS. Designers want 3D pieces and dice rendered with RealityKit, synchronous play over FaceTime, and optional Game Center features such as achievements or matchmaking. A reviewer is worried the proposal may mix rendering, networking, and game-state authority in ways that will be hard to maintain.

Write an architecture note that defines the responsibility boundaries between TabletopKit, RealityKit, Group Activities/SharePlay, and GameKit. Include practical implementation guidance for seats, turns, rendering updates, multiplayer synchronization, and dice/card interactions where relevant.

## Output Specification

Create `tabletopkit-multiplayer-architecture.md` with concise guidance, a small responsibility table, and a review checklist. Do not create an Xcode project.
