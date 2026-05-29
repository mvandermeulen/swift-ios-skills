# SwiftLint Plugin and CI Setup

## Problem/Feature Description

A team is adding SwiftLint to a new iOS app that has both SwiftPM package targets and Xcode app targets. They want local linting during builds, a pinned or reviewed SwiftLint version, GitHub Actions output that can be uploaded as SARIF, and safe guidance for unattended CI builds that use `xcodebuild`.

## Output Specification

Create `swiftlint-plugin-ci-setup.md` with:

- the recommended local integration path,
- the essential `Package.swift` or Xcode target setup snippets,
- a GitHub Actions SARIF reporting snippet,
- plugin trust and unattended CI caveats,
- no generated Xcode project.
