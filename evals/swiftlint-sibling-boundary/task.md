# Swift Cleanup Routing

## Problem/Feature Description

A package maintainer is triaging three cleanup requests before assigning issues:

1. choose better public API names for `func fetchDataWithId(_ id: String)`,
2. decide whether `some` or `any` is right for a protocol return type,
3. configure linting to enforce identifier naming and sorted imports.

They want one short routing memo that says which domain owns each concern and gives only the minimum concrete examples needed.

## Output Specification

Create `swiftlint-cleanup-routing.md` containing:

- a brief owner/domain for each cleanup item,
- a minimal API naming example,
- a minimal SwiftLint configuration example,
- no full `.swiftlint.yml`, no protocol type-system tutorial, and no package scaffolding.
