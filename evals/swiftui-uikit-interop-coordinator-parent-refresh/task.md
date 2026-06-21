# SwiftUI/UIKit Search Bar Coordinator Review

## Problem/Feature Description

A SwiftUI app wraps a legacy `UISearchBar`:

```swift
struct SearchBar: UIViewRepresentable {
    @Binding var text: String
    var onSearch: (String) -> Void

    func makeCoordinator() -> Coordinator { Coordinator(self) }

    func makeUIView(context: Context) -> UISearchBar {
        let bar = UISearchBar()
        bar.delegate = context.coordinator
        return bar
    }

    func updateUIView(_ uiView: UISearchBar, context: Context) {
        if uiView.text != text { uiView.text = text }
    }

    final class Coordinator: NSObject, UISearchBarDelegate {
        var parent: SearchBar
        init(_ parent: SearchBar) { self.parent = parent }

        func searchBarSearchButtonClicked(_ searchBar: UISearchBar) {
            parent.onSearch(parent.text)
        }
    }
}
```

Review the wrapper for correctness under SwiftUI/UIKit interop.

## Output Specification

Create `swiftui-uikit-interop-coordinator-review.md` with:

- The corrected coordinator refresh pattern.
- Where delegate assignment belongs.
- How to avoid redundant SwiftUI-to-UIKit update loops.
- How UIKit user edits should write back to SwiftUI state.
- Why copied coordinator state can go stale.
