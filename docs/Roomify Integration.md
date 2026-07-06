# **Roomify Integration**

Securify works as a standalone Indigo plugin.

It does not require Roomify.

When Roomify is installed, however, the two plugins can cooperate.

That cooperation allows the home to share higher-level context between comfort, occupancy, lighting, awareness, and response.

Roomify helps the home understand how it should behave.

Securify helps the homeowner understand when something deserves attention.

Together, they support a home that adapts to its occupants while remaining aware of changing conditions.

---

# **Different Responsibilities**

Roomify and Securify have different purposes.

**Roomify accommodates.**

It adapts rooms to changing occupancy, House Mode, lighting expectations, and homeowner intent.

**Securify informs.**

It interprets conditions that may deserve awareness and, when authorized, responds according to homeowner policy.

Roomify is not a security system.

Securify is not a room automation system.

Each plugin remains responsible for its own domain.

---

# **Shared House Mode**

The primary integration point is House Mode.

Roomify can provide the current House Mode to Securify.

Securify can then use that House Mode to adjust Watchfulness automatically.

For example:

- Day mode may use lower Watchfulness.
- Evening mode may use moderate Watchfulness.
- Bedtime may use high Watchfulness.
- Sleep or Away mode may use maximum Watchfulness.

This allows Securify to become more or less sensitive as the home moves through normal daily patterns.

---

# **Watchfulness and Context**

Watchfulness is Securify’s primary expression of context.

Roomify helps provide that context by describing the current operating state of the home.

The same condition may therefore be interpreted differently depending on the mode Roomify has established.

An unlocked door during Day mode may be relatively insignificant.

The same unlocked door during Sleep mode may deserve immediate attention.

Roomify does not decide whether the condition matters.

It helps Securify understand the current household context so Securify can apply the homeowner’s policy appropriately.

---

# **Roomify Occupancy Checkpoints**

When integration is enabled, Roomify occupancy can be used as a Securify checkpoint type.

This allows Securify to interpret higher-level occupancy rather than relying only on raw motion signals.

A room being occupied may carry different meaning depending on Watchfulness and House Mode.

For example:

- occupancy in a common room during Day mode may be normal
- occupancy in a room during Away mode may deserve concern
- unexpected occupancy at night may warrant awareness

Roomify determines occupancy.

Securify determines whether that occupancy represents a condition of concern.

---

# **Separate Decisions**

Roomify and Securify may both respond to the same household context, but they do so for different reasons.

Roomify might adjust lighting because a room has become occupied.

Securify might increase concern because occupancy occurred while the house was expected to be vacant.

Those are not competing decisions.

They are different interpretations of the same reality.

Roomify adapts the home.

Securify informs the homeowner.

---

# **Optional Cooperation**

Roomify integration is optional.

Homeowners may use:

- Securify by itself
- Roomify by itself
- both plugins together

When both are installed, cooperation improves context.

When only Securify is installed, Watchfulness and checkpoints still operate normally.

Securify remains fully functional as an independent awareness engine.

---

# **Open Indigo Integration**

Both Roomify and Securify publish meaningful Indigo device states.

Because those states are available throughout Indigo, homeowners remain free to create their own triggers, conditions, Action Groups, variables, dashboards, and scripts that combine the two systems in any way they choose.

The plugins provide structure.

Indigo provides openness.

The homeowner remains in control.

---

# **A Shared Philosophy**

Roomify and Securify are built around the same philosophy.

The homeowner defines intent.

Roomify accommodates that intent by adapting the home.

Securify protects that intent by revealing conditions that deserve attention.

Together, they move the smart home away from simple device reaction and toward a more meaningful model:

- The homeowner decides.
- Roomify accommodates.
- Securify informs—and, when configured, responds.

Everything else follows from those principles.

![](/docs/images/SecurifyLogo200.png)
