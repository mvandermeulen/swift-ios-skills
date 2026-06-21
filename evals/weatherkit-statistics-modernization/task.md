# WeatherKit Statistics Modernization

## Problem/Feature Description

A developer wants to update an older WeatherKit historical statistics snippet for modern iOS targets:

```swift
let stats = try await service.dailyStatistics(
    for: location,
    forDaysIn: range,
    including: [.temperature, .precipitation]
)

for day in stats {
    print(day.statistics(for: .temperature)?.mean)
}
```

They also need a monthly statistics example for the same app.

## Output Specification

Create `weatherkit-statistics-modernization.md` with corrected daily and monthly WeatherKit statistics examples and a short migration explanation. Keep the focus on WeatherKit statistics APIs rather than charting or generic data modeling.
