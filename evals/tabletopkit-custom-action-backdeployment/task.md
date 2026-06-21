# TabletopKit Custom Action Backdeployment Review

## Problem/Feature Description

A teammate proposes adding a custom "claim route" move and custom per-piece state to a TabletopKit strategy game. The product target includes visionOS 2.x devices, but the prototype uses newer TabletopKit APIs for custom actions, custom equipment state, and custom action registration.

Review the proposal and write guidance that keeps the implementation correct across visionOS 2.0, 2.2, and 26. The review should explain which APIs can be used directly, which must be availability-gated, and how to keep game actions deterministic for multiplayer.

## Output Specification

Create `tabletopkit-custom-action-review.md` with a concise technical review, Swift snippets or pseudocode where helpful, and a final migration checklist. Do not create an Xcode project.
