# **Plugin Coordination**

Beginning with the 1.x generation, SearchCz plugins can optionally coordinate with one another.

Each plugin remains completely functional on its own. Coordination is never required.

When enabled by the homeowner, compatible SearchCz plugins exchange high-level requests, suggestions, and information through well-defined callback methods. Every interaction is optional, and every receiving plugin decides whether the request should be honored according to its own configuration and homeowner preferences.

This architecture keeps plugins loosely coupled while allowing them to behave as a unified home automation system.

## **Examples**

### **Shared House Mode**

Roomify and Securify both understand the concept of House Mode.

If coordination is enabled in both plugins, a House Mode change initiated by either plugin can be suggested to the other. The receiving plugin evaluates the suggestion and, if appropriate, adopts the same mode.

Whether House Mode is changed manually, by automation, or by another SearchCz plugin, the homeowner can choose to keep both plugins synchronized automatically.

### **Security-Aware Rooms**

When Securify determines that a checkpoint protecting a room has become vulnerable, it can inform Roomify of the room’s current security exposure.

Roomify immediately reflects that condition in the associated Room device, allowing Indigo automations and user interfaces to understand not only occupancy and authority, but also the room’s current security state.

This creates a shared semantic model where occupancy, lighting, automation authority, and security awareness all describe the same room.

### **Information Sharing**

Plugins may also exchange information without requesting any action.

For example, Securify may ask Roomify for its current House Mode when evaluating homeowner-defined security policies.

Other SearchCz plugins may expose similar capabilities as the ecosystem grows.

## **Homeowner Control**

Plugin coordination is always optional.

Each compatible plugin includes a configuration option allowing the homeowner to participate—or not participate—in coordination with other SearchCz plugins.

A plugin that is not configured for coordination simply ignores incoming requests and continues operating independently.

## **Designed for Growth**

The coordination framework is intentionally generic.

Today’s interactions include House Mode synchronization and room security awareness.

Future SearchCz plugins will be built to exchange requests, suggestions, notifications, and information using the same coordination model without introducing tight dependencies between plugins.

The result is a collection of independent plugins that can, when desired, work together as a coherent automation platform.

*Roomify 1.3.x or higher required for plugin coordination*

![](/docs/images/SecurifyLogo200.png)
