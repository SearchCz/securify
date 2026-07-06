# **Observers**

An **Observer** is an Indigo device that the homeowner creates to watch for a particular security condition and, when appropriate, respond to it.

Where checkpoints interpret the home, observers interpret the checkpoints.

A checkpoint continuously evaluates the significance of a condition.

An observer decides whether that condition deserves the homeowner’s attention.

---

# **Purpose**

Observers separate **awareness** from **response**.

A single checkpoint may represent an unlocked door, a water leak, or unexpected motion.

Whether that condition deserves an announcement, an email, a Pushover notification, or no response at all depends entirely on the homeowner’s priorities.

Observers allow those decisions to be expressed independently of the checkpoint itself.

This separation keeps checkpoints simple while allowing multiple observers to react differently to the same condition.

---

# **Three Responsibilities**

Every observer performs three distinct functions.

## **Focus**

An observer first defines **what it is watching**.

Its focus may be:

- a specific checkpoint
- the home as a whole
- a condition becoming more significant
- a condition becoming less significant
- a condition reaching a particular Alert Classification

When an observer’s focus is satisfied, the observer becomes **active**.

Its Indigo device turns on, indicating that the condition it watches currently exists.

Activation does not necessarily produce a notification.

It simply means the observed condition is present.

---

## **Authority**

Once active, an observer determines whether it is currently authorized to respond.

Authorization allows homeowners to suppress unwanted noise without changing what the observer is watching.

Examples include:

- requiring the condition to persist for a period of time
- requiring a homeowner-defined gating device to be true
- combining both persistence and gating requirements

An observer may therefore remain active for some time before it becomes authorized to respond.

---

## **Response**

When both the observer’s focus and authority requirements have been satisfied, the observer performs one or more homeowner-defined responses.

Responses may include:

- spoken announcements
- email notifications
- Pushover notifications
- Indigo Action Groups
- Indigo Variables

Responses may also be repeated according to homeowner-defined schedules for as long as authorization continues.

---

# **Independent Observers**

Observers do not compete with one another.

Multiple observers may watch the same checkpoint simultaneously.

For example, one observer might announce that a garage door has been left open after five minutes.

Another might send an email after thirty minutes.

A third might execute an Indigo Action Group after two hours.

Each observer has its own focus, authority, and response policy.

Because these responsibilities are independent, sophisticated notification strategies can be built without changing the underlying checkpoint.

---

# **Observers Are Indigo Devices**

Like checkpoints, observers are ordinary Indigo devices.

Their current state is published throughout Indigo and may be used by any trigger, condition, or Action Group.

An observer turning on simply indicates that the condition it watches currently exists.

Whether Securify responds to that condition—or whether Indigo responds through custom automation—is entirely up to the homeowner.

---

# **A Layer of Awareness**

Observers are where interpretation becomes awareness.

Checkpoints determine the significance of changing conditions.

Observers determine which of those conditions deserve attention.

Together they allow Securify to continuously interpret the home while ensuring that responses remain consistent with the homeowner’s priorities.