A home-automation app is implementing a Control Center garage-door toggle.

The draft uses:

- `ControlWidgetToggle(isOn:action:)` with a plain parameterless `AppIntent`.
- A value provider that reads cached state, but the intent returns before saving the requested state.
- `ControlPushHandler.pushTokensDidChange(controls: [ControlPushInfo])`.
- Remote APNs pushes with `apns-push-type: widgets` and a custom JSON body containing the new open/closed state.

Review the plan and provide the corrected WidgetKit controls shape with a compact Swift sketch.
