# 5.4. Notification System

This section describes the minimum notification system requirements.

## Communication Channels

Application will communicate with members via two delivery mechanism:

* **email notifications** \(Xxxxxxxxxxxxxxxxxx\)
* **push notifications** \(Firebase Cloud Messaging\)

### Notification Strategy

Application will use two types of notifications: the Notice and the Reminder.

* **Notice** A notice is one time event.
* **Reminder** A reminder is a reccuring event.

Notifications can be triggered in two ways:

* **automatically** - by application
* **manually** - by user input, de facto a message to targeted group. For example: admin wants to send a message to all subscribed volunteers.

**If opted-in a member will receive notification in case of:**

| Notification | Push | Email |  | Type |  | Triggered by |  | Supporter | Sponsor | Volunteer |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| New Sponsor Event Announcement |  |  |  | Notice |  | Application |  |  | Yes |  |
| New Sponsor Event Activated | Yes |  |  | Notice |  | Application |  |  | Yes |  |
| Standing Instruction Expired | Yes |  |  | Notice |  | Notice |  | Yes | Yes |  |
| Protege Thanks Note | Yes | Yes |  | Notice |  | Notice |  |  | Yes |  |
| Protege Additional Need | Yes | Yes |  | Notice |  | Notice |  |  | Yes |  |
| New Volunteer Event Announcement | Yes | Yes |  | Notice |  | Notice |  |  |  | Yes |
| New Volunteer Event Activated | Yes | Yes |  | Notice |  | Notice |  |  |  | Yes |
| Organization Operational Need | Yes | Yes |  | Notice |  | Notice |  |  |  | Yes |

> This is not a full list of notifications.

### Managing Notification Subscriptions

A member has total control over notifications from hers/his profile page.

**A logged-in member can enable/disable:**

* all notifications.
* a single notification.

### Notification Page

### Notification Widget

### Upcoming Events

