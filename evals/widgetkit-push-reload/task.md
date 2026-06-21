A team is adding iOS 26 server-driven freshness for an order-status Home Screen widget.

Their draft plan:

- Put a `WidgetPushHandler` type in the main app target.
- Register for push notifications with the User Notifications framework.
- Send APNs broadcast channel pushes whenever an order changes.
- Use the push as the widget's primary freshness model and keep the timeline provider minimal.
- Skip app-side `WidgetCenter` reloads because the server will send every update.

Write a concise review that corrects the WidgetKit architecture and names the concrete API/header details the implementation should use.
