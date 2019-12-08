# 5.4. Notification System

This section describes the minimum notification system requirements.

## Communication Channels

Application will communicate with members utilizing two delivery mechanisms:

* **email notifications** via SendGrid.
* **push notifications** via Firebase Cloud Messaging.

### Notification Strategy

Application will use two types of notifications: **Notices and Reminders**.

* **Notice**

  A notice is one time event.

* **Reminder**

  A reminder is a reccuring event.

Notifications can be triggered in two ways:

* **automatically**

  Triggered by application.

* **manually**

  Triggered by user input, de facto a message to targeted group.

  For example: admin wants to send a message to all subscribed volunteers.

**If opted-in a member will receive notification in case of:**

| Notification | Push | Email |  | Type |  | Triggered by |  | Supporter | Sponsor | Volunteer |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| New Sponsor Event Announcement |  |  |  | Notice |  | Application |  |  | Yes |  |
| New Sponsor Event Activated | Yes |  |  | Notice |  | Application |  |  | Yes |  |
| Standing Instruction Expired | Yes |  |  | Reminder |  | Application |  | Yes | Yes |  |
| Protege Thanks Note | Yes | Yes |  | Notice |  | Application |  |  | Yes |  |
| Protege Additional Need | Yes | Yes |  | Notice |  | Application |  |  | Yes |  |
| New Volunteer Event Announcement | Yes | Yes |  | Notice |  | Application |  |  |  | Yes |
| New Volunteer Event Activated | Yes | Yes |  | Notice |  | Application |  |  |  | Yes |
| Volunteer Subscribed Event Reminder | Yes | Yes |  | Reminder |  | Application |  |  |  | Yes |
| Organization Operational Need | Yes | Yes |  | Notice |  | Admin, Staff |  |  |  | Yes |

> This is not a full list of notifications.

### Notification Types

> Events by notification types.

| Event | Notice | Reminder |
| :--- | :--- | :--- |
| _Budget 2020_ | Yes |  |
| _Volunteers Wanted_ |  |  |
| _Hands-on \#34_ |  | Yes |
| _Sponsors Wanted_ | Yes |  |
| _Christmas Gift_ |  | Yes |
| _Easter Gift_ |  | Yes |
| _Birthday Presents for January_ |  | Yes |
| _Back to School_ |  | Yes |
| _Vacation Summer_ |  | Yes |

### Managing Notification Subscriptions

A member has total control over notifications from hers/his profile page.

A logged-in member can **enable/disable**:

* **all notifications**
* **single notification**

### Upcoming Events Reminder

A member can subscribe/unsubscribe to a certain upcoming event @upcoming events widget.

> Should be discussed with a developer.

### The Smart Bar

A visitor/member can subscribe to an actual event via the Smart Bar.

The Smart Bar is a front-end \(PWA\) global messaging subsystem with reccuring reminder on top of the screen.

It is bound to an Event and it alerts all visitors/members about current time status of the event.

Content/messages of the Smart bar are created and controlled within the event.

> Should be discussed with a developer.

