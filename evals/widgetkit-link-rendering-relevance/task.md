A widget design note contains these claims:

- A small system widget can only use `widgetURL(_:)`; `Link` starts at medium widgets.
- Liquid Glass support is handled by choosing one `WidgetAccentedRenderingMode` case for the whole widget.
- An iPhone Smart Stack should use `AppIntentTimelineProvider.relevance()` and return `WidgetRelevance(intent, score: 80)`.
- The answer should include whatever ActivityKit and App Intents details are needed.

Rewrite the note so it is correct for current WidgetKit, but keep the scope focused on the widget design and implementation boundaries.
