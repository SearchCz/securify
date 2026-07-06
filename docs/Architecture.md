# **Architecture**

Securify is built as a layered awareness pipeline.

Each layer has one responsibility.

Devices report facts.

Checkpoints interpret those facts.

Observers determine whether interpreted conditions deserve attention.

Responses inform the homeowner or trigger Indigo automation.

---

# **Awareness Pipeline**

```text
Binary Device Signals
        │
        ▼
   Checkpoints
 interpret meaning
        │
        ▼
 Significance
 Brightness 0–100
 Alert Classification
        │
        ▼
    Observers
 Focus → Authority → Response
        │
        ▼
 Homeowner Awareness
 Indigo Automation
```

---

# **Layer Responsibilities**

## **Devices**

Devices provide raw facts.

They may report conditions such as:

- open or closed
- locked or unlocked
- motion or no motion
- occupied or vacant
- leak detected or clear

Securify does not ask these devices to decide what their state means.

---

## **Checkpoints**

Checkpoints are homeowner-defined Indigo devices.

They interpret raw device states in the context of:

- homeowner-defined importance
- signal persistence
- current Watchfulness

Each checkpoint publishes its current significance as Indigo device state, including Brightness on a 0–100 scale and Alert Classification.

---

## **Observers**

Observers are homeowner-defined Indigo devices that watch checkpoints or the home as a whole.

Each observer has three parts:

- **Focus** — what condition it watches
- **Authority** — when response is permitted
- **Response** — what happens when authorized

When an observer’s Focus is met, the observer turns **On**.

Turning On represents awareness, not notification.

---

## **Responses**

Responses occur only when an observer is both active and authorized.

Responses may include:

- announcements
- email
- Pushover
- Indigo Action Groups
- Indigo Variables
- repeated responses

Responses do not decide whether a condition matters.

They simply carry out the observer’s configured policy.

---

# **Separation of Responsibilities**

Securify intentionally separates interpretation from response.

A checkpoint never notifies.

An observer’s activation does not necessarily notify.

A response never decides whether it should occur.

This keeps the system predictable.

```text
Checkpoint = What does this condition mean?
Observer Focus = Does the watched condition exist?
Observer Authority = Is response permitted?
Observer Response = How should the homeowner be informed?
```

---

# **Multiple Observers**

Multiple observers may watch the same checkpoint.

This allows one checkpoint to support many response policies.

For example:

```text
Garage Door Checkpoint
        │
        ├── Observer: Announce after 5 minutes
        ├── Observer: Email after 30 minutes
        └── Observer: Pushover at critical significance
```

The checkpoint calculates significance once.

Each observer decides independently whether and how to respond.

Observers do not escalate.

Conditions escalate.

---

# **Indigo Openness**

Checkpoints and observers are ordinary Indigo devices.

Their states are available throughout Indigo and may be used in homeowner-created triggers, conditions, Action Groups, variables, dashboards, and scripts.

Securify provides an opinionated awareness engine, but it does not close off Indigo’s native automation model.

The homeowner remains free to build on top of the semantic state Securify publishes.

---

# **Design Principle**

Securify’s architecture follows one guiding idea:

**The homeowner decides what deserves attention.**

Everything else exists to apply that decision consistently.

Devices report.

Checkpoints interpret.

Observers authorize.

Responses inform.

![](/docs/images/SecurifyLogo200.png)
