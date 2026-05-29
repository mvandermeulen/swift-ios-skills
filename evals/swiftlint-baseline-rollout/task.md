# SwiftLint Existing-Codebase Rollout

## Problem/Feature Description

A large existing Swift app has thousands of current SwiftLint violations. The maintainers want to adopt SwiftLint without blocking every pull request on legacy issues. They also need guidance for intentional exceptions, generated code, and test code that uses force unwraps in fixtures.

## Output Specification

Create `swiftlint-rollout-plan.md` containing:

- a phased adoption plan,
- the relevant `.swiftlint.yml` and CI command snippets,
- suppression policy for intentional exceptions,
- generated-code and test-target handling,
- no package scaffolding.
