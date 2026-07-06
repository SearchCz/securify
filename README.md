# **Securify**

![/[docs/images/SecurifyBanner.png]]

**Awareness-driven home monitoring for Indigo Domotics**

A smart home should do more than react to devices.

It should understand the people who live there, adapt to their priorities, and keep them aware of the conditions that matter.

That philosophy places the homeowner—not the automation—at the center of the system.

- The homeowner defines priorities and policies.
- Roomify accommodates.
- Securify informs—and, when configured, responds.

Everything else follows from those principles.

---

## **Why Securify?**

Traditional alarm systems are designed to detect emergencies.

Securify is designed to reveal conditions that deserve your attention—often long before they become emergencies.

An unlocked door at bedtime.

A garage left open.

A water leak that has persisted for thirty minutes.

Unexpected motion while the home should be empty.

None of these situations necessarily requires an alarm, but each may warrant awareness depending on your priorities, the current state of your home, and how long the condition has persisted.

Securify continuously interprets the home’s condition so that you can decide what deserves your attention.

---

## **Not an Alarm System**

Securify doesn’t compete with your alarm system. It occupies the space around it.

Your alarm system is there for the moments that demand an immediate response.

Securify is there for the many other moments that deserve your awareness because of context, persistence, or homeowner-defined priorities.

Rather than asking whether a sensor is simply _on_ or _off_, Securify continually evaluates what that state means.

---

## **How It Works**

At the heart of Securify are two concepts.

### **Checkpoints**

Checkpoints interpret one or more binary signals and determine their current significance.

A checkpoint considers:

- the importance assigned by the homeowner
- the current watchfulness of the home
- how long a condition has persisted

The result is an evolving assessment of concern rather than a simple binary state.

### **Observers**

Observers watch for meaningful security conditions.

When a condition of interest occurs—and any persistence or authorization requirements have been satisfied—an observer can respond by:

- making an announcement
- sending an email
- delivering a Pushover notification
- executing an Indigo Action Group
- updating an Indigo Variable
- repeating responses according to homeowner policy

---

## **Watchfulness**

Every home experiences different levels of vulnerability throughout the day.

Securify models this using **Watchfulness**.

Watchfulness represents how alert the home should be under current circumstances.

For example:

- Daytime at home may require relatively low watchfulness.
- Bedtime may significantly increase watchfulness.
- Away mode may represent the highest watchfulness.

As watchfulness changes, the same sensor condition may become more—or less—worthy of your attention.

---

## **Designed to Work with Roomify**

Roomify and Securify were designed together.

Roomify helps the home understand how it should behave.

Securify helps the homeowner understand when something deserves attention.

Together they create a home that both adapts to its occupants and remains aware of conditions that matter.

Neither plugin depends on the other, but when both are installed they cooperate by sharing information such as House Mode and occupancy, allowing each plugin to make better decisions.

---
## **Philosophy**

Securify is built on a simple principle:

The homeowner—not the automation—decides what deserves attention.

Securify continuously interprets the home’s condition, quietly filters everyday noise, and reveals the situations that matter most.!

---
## **Documentation**

Detailed documentation is available in the **docs** folder.

- [Overview](docs/Overview.md)
- [Watchfulness Configuration](docs/Watchfulness.md)
- [Checkpoints](docs/Watchfulness)
- [Observers](docs/Observer%20Overview.md)
- [Observer Focus](docs/Observer%20Focus.md)
- [Observer Authority](docs/Observer%20Authority.md)
- [Observer Responses](docs/Obserever%20Responses.md)
- [Roomify Integration](docs/Roomify%20Integration.md)

---


![[SecurifyLogo200.png]]
