# **Observer Responses**

An observer’s **Response** defines how the homeowner should be informed once the observer has become authorized.

Focus determines what the observer watches.

Authority determines when it is permitted to respond.

Response determines what happens next.

By separating these responsibilities, Securify allows homeowners to change how they are informed without changing what they are watching or when responses are authorized.

---

# **One Observer,  Many Responses**

A single observer may perform one or more responses.

For example, an observer might:

- announce a message throughout the home
- send an email
- deliver a Pushover notification
- execute an Indigo Action Group
- update an Indigo Variable

These responses may occur individually or in any combination.

The observer simply performs every response that has been configured.

---

# **Announcements**

Announcements provide immediate spoken feedback through Indigo.

They are well suited to situations where someone is already at home and can act immediately.

Examples include:

- “The garage door has been open for fifteen minutes.”
- “The front door is unlocked.”
- “Water has been detected in the utility room.”

Homeowners may choose the level of detail appropriate for each announcement.

---

# **Email**

Email responses provide a permanent record of conditions that deserve attention.

They are particularly useful for conditions that may require later review or that occur while the homeowner is away.

---

# **Pushover**

Pushover notifications deliver immediate alerts to one or more mobile devices.

Each observer may define its own notification priority and destination devices, allowing different conditions to be delivered with different levels of urgency.

---

# **Indigo Action Groups**

Observers may execute any Indigo Action Group when they become authorized.

This allows Securify to integrate naturally with the rest of an Indigo automation system.

Examples include:

- turning on exterior lighting
- sounding a chime
- activating another automation
- notifying another plugin
- triggering custom workflows

Securify does not dictate how the home should respond.

It simply provides the opportunity.

---

# **Indigo Variables**

Observers may also assign information to an Indigo Variable.

Variables allow other automations to react to changing security conditions or to display those conditions elsewhere within Indigo.

This provides a simple mechanism for integrating Securify with dashboards, control pages, scripts, and other plugins.

---

# **Repeating Responses**

Some conditions deserve repeated reminders until they are resolved.

Observers may therefore repeat their configured responses according to a homeowner-defined schedule.

For example, an observer might announce that a garage door remains open every fifteen minutes until it is closed.

Repeating responses continue only while the observer remains authorized.

As soon as the observed condition is resolved—or Authority is withdrawn—repeating responses stop automatically.

---

# **Responses Do Not Escalate**

An observer’s response is fixed.

It does not become more urgent over time.

If a homeowner wishes to respond differently as a condition becomes more significant, they simply create additional observers with different Focus, Authority, and Response configurations.

For example:

- One observer announces that the garage door has been left open.
- Another sends an email if the condition becomes more serious.
- A third delivers a high-priority Pushover notification if the condition reaches a critical level.

Each observer performs a single, well-defined job.

This keeps the system simple, predictable, and easy to understand.

---

# **Integration with Indigo**

Responses are intentionally open-ended.

While Securify provides several built-in response mechanisms, Indigo Action Groups and Variables make it possible to integrate Securify with virtually any automation supported by Indigo.

The homeowner remains free to decide how the home should react to changing conditions.

Securify simply ensures those reactions occur at the appropriate time.

---

# **Inform, Then Respond**

The primary purpose of Securify is awareness.

Every response exists to keep the homeowner informed of conditions that deserve attention.

Whether that awareness takes the form of a spoken announcement, an email, a mobile notification, or a custom automation is entirely the homeowner’s choice.

Securify interprets the home.

Observers decide when a response is appropriate.

Responses simply deliver the message.

![[SecurifyLogo200.png]]