# **Watchfulness Configuration**

Watchfulness is the heart of Securify.

It represents how alert the home should be at any given moment and directly influences how significant a condition is considered to be.

An unlocked door, for example, may be of little concern while the homeowner is working in the yard. The same door may deserve immediate attention after everyone has gone to bed.

Rather than changing the condition itself, Watchfulness changes how that condition is interpreted.

---

# **Dynamic Watchfulness**

In most homes, vulnerability changes throughout the day.

Securify embraces this idea by allowing Watchfulness to change automatically as the home’s operating mode changes.

Typical examples include:

|**House Mode**|**Typical Watchfulness**|
|---|---|
|Morning|Moderate|
|Day|Low|
|Evening|Moderate|
|Bedtime|High|
|Sleep|Very High|
|Away|Maximum|

These are not fixed values.

Every homeowner has different expectations, and every home has different routines.

---

# **Opinionated Defaults**

Securify includes a set of sensible default Watchfulness levels.

These defaults reflect a common expectation that:

- occupied homes are generally less vulnerable than unoccupied homes
- sleeping occupants are more vulnerable than awake occupants
- away mode typically requires the greatest awareness

These defaults are intended as a starting point, not a rule.

---

# **Homeowner Overrides**

Every House Mode can be assigned its own Watchfulness level.

You are free to adjust these values to reflect how your household operates.

For example, some homeowners may prefer Away mode and Sleep mode to have identical Watchfulness, while others may intentionally make Sleep even more sensitive because occupants are less likely to notice changing conditions.

Securify simply applies the policy you define.

---

# **Cooperation with Roomify**

When Roomify is installed, both plugins can share House Mode information.

As Roomify changes the operating mode of the home, Securify automatically adjusts Watchfulness to match.

No additional automation is required.

Although this integration is seamless, it is entirely optional.

Securify works perfectly well as a standalone plugin.

---

# **Logging**

Securify provides several logging options to assist with troubleshooting and understanding system behavior.

Logging can be enabled for areas such as:

- checkpoint evaluation
- observer activity
- responses
- heartbeat processing
- other diagnostic information

Most homeowners will never need detailed logging during normal operation.

Diagnostic logging is primarily intended for installation, troubleshooting, and plugin development.

---

# **A Design Philosophy**

Many security systems define fixed rules.

Securify defines a moving context.

Instead of asking:

“Is this condition dangerous?”

Securify asks:

“Given the current state of the home, how concerned should the homeowner be?”

Watchfulness provides the context that allows the same physical condition to be interpreted differently as the home changes throughout the day.

It is one of the defining ideas behind Securify’s awareness-driven design.

![](/docs/images/SecurifyLogo200.png)
