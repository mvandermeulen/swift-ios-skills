# Vision Framework Modern API Boundary Review

## Problem

An iOS 26 app team is reviewing a mixed Vision helper for receipts and camera
frames. The draft does all of the following:

- Uses `DetectBarcodesRequest` but configures it with `[VNBarcodeSymbology]`.
- Stores every modern Vision `boundingBox` as `CGRect` and converts it with
  `VNImageRectForNormalizedRect`.
- Starts object tracking with `TrackObjectRequest(observation:)` and sets
  `trackingLevel`.
- Calls `generateMask(forInstances:)` on an `InstanceMaskObservation`.
- Treats horizon and saliency request results as arrays and reads `first`.
- Uses `DataScannerViewController` for a SwiftUI live QR/text scanner but only
  checks `isSupported`.
- Optionally runs a custom Core ML classifier through Vision and starts adding
  model conversion and deployment notes to the Vision helper.

Review the draft and provide corrected Swift snippets and boundary guidance.

## Output

Create a Markdown file named `vision-framework-modern-api-boundary.md`.

Keep the answer focused on Vision and VisionKit implementation guidance. Do not
create an Xcode project, and do not expand into Core ML conversion, profiling,
or deployment implementation.
