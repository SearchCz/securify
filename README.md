# **Securify**

![](/docs/images/SecurifyBanner.png)

**Awareness-driven home monitoring for Indigo Domotics**

Most home automation systems know **what happened**.

Securify determines **what deserves your attention**.

Rather than treating every sensor equally, Securify continuously evaluates household conditions using homeowner-defined priorities, the home's current watchfulness, and the passage of time. The result is fewer meaningless notifications—and greater awareness of the conditions that actually matter.

---

## **Why Securify?**

Securify doesn't compete with your alarm system. It occupies the space around it.

Traditional alarm systems exist for emergencies.

Securify exists for everything else that may deserve your awareness.

An unlocked door at bedtime.

A garage left open.

A water leak that's been dripping for thirty minutes.

Unexpected motion while the house should be empty.

None of these situations necessarily requires an alarm. Their significance depends on context.

Securify continuously interprets that context so the homeowner—not the automation—decides what deserves attention.

---

## **A Different Philosophy**

A smart home should do more than react to devices.

It should understand the people who live there, adapt to their priorities, and keep them aware of the conditions that matter.

That philosophy places the homeowner—not the automation—at the center of the system.

- The homeowner defines priorities and policies.
- Roomify accommodates.
- Securify informs—and, when configured, responds.

Everything else follows from those principles.

---

## **How Securify Thinks**

Instead of asking whether a sensor is simply *on* or *off*, Securify continually asks:

> **"How significant is this condition right now?"**

That significance changes throughout the day.

A door left unlocked at noon may be perfectly acceptable.

The same unlocked door at bedtime may deserve immediate attention.

A small water leak that has existed for two minutes may not matter.

After an hour, it probably does.

Securify continuously re-evaluates these conditions as your home's circumstances change.

---

## **Checkpoints**

Checkpoints are where raw device signals become meaningful information.

A checkpoint combines one or more binary sensor states with:

- Homeowner-defined importance
- Current Watchfulness
- Persistence over time

The result is a continuously changing **Brightness** score (0–100) that represents the current significance of the condition.

Rather than producing a simple *safe/not safe* result, checkpoints express how worthy of attention each condition has become.

---

## **Watchfulness**

Every home experiences changing levels of vulnerability.

Securify models this using **Watchfulness**.

Watchfulness represents how alert the home should be under current circumstances.

For example:

- Home during the day may use relatively low watchfulness.
- Bedtime may significantly increase watchfulness.
- Away mode may represent maximum watchfulness.

As Watchfulness changes, checkpoint Brightness changes automatically—even when the underlying sensor hasn't changed.

---

## **Observers**

Observers watch for conditions the homeowner cares about.

Each observer defines its own **Focus** by selecting the range of checkpoint Brightness values it considers important.

Multiple observers can watch the same checkpoint simultaneously, each looking for different levels of concern and responding differently.

When an observer's focus is satisfied—and any persistence or authorization requirements have been met—it activates and can:

- Make announcements
- Send email
- Deliver Pushover notifications
- Execute Indigo Action Groups
- Update Indigo Variables
- Repeat responses according to homeowner policy

Observers don't decide what's important.

They simply respond to the homeowner's definition of importance.

---

## **Designed to Work with Roomify**

Roomify and Securify were designed together.

Roomify helps the home understand how it should behave.

Securify helps the homeowner understand what deserves attention.

When both plugins are installed they share information—including House Mode and occupancy—allowing each plugin to make better decisions.

Neither plugin depends on the other.

---

## **Philosophy**

Securify is an awareness engine.

It doesn't decide what to do.

It recognizes when your priorities indicate that a condition deserves attention and works to ensure you know about it.

The homeowner decides.

Securify watches.

---

## **Documentation**

Detailed documentation is available in the **docs** folder.

- [Overview](docs/Overview.md)
- [Watchfulness](docs/Watchfulness.md)
- [Checkpoints](docs/Checkpoints.md)
- [Observers](docs/Observer%20Overview.md)
- [Observer Focus](docs/Observer%20Focus.md)
- [Observer Authority](docs/Observer%20Authority.md)
- [Observer Responses](docs/Observer%20Responses.md)
- [Roomify Integration](docs/Roomify%20Integration.md)

---

![](/docs/images/SecurifyLogo200.png)

![[SecurifyLogo200.png]]
