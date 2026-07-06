# **Checkpoints Produce Information**

A checkpoint’s responsibility is interpretation.

It continuously evaluates the significance of a condition and publishes that interpretation as the state of an Indigo device.

Checkpoints never send notifications, execute Action Groups, or otherwise decide how the home should respond.

That responsibility belongs to Observers—or to the homeowner.

Because every checkpoint is an ordinary Indigo device, its states are available throughout Indigo. Homeowners are free to create their own triggers, conditions, and Action Groups that respond to changes in checkpoint states exactly as they would for any other Indigo device.

Some homeowners may choose to build their own custom automations around checkpoint state changes. Others may rely entirely on Securify’s Observer framework. Many will use both.

Observers provide a powerful, integrated way to respond to changing security conditions, but they are entirely optional.

By separating interpretation from response, Securify remains flexible while fitting naturally into Indigo’s event-driven automation model.

# **Alert Classification and Brightness**

Every checkpoint continuously evaluates its current condition and produces an **Alert Classification**, representing the current significance of that condition.

To make that significance immediately visible, each checkpoint also publishes a **Brightness** value between **0 and 100**.

Brightness is a continuously changing representation of the checkpoint’s current level of concern.

- **0** represents a completely unconcerning condition.
- **100** represents the maximum significance that checkpoint can currently express.
- Intermediate values reflect changing significance as persistence, watchfulness, and device state evolve.

For example, a garage door may begin with relatively low significance when first opened. As time passes, its Brightness may gradually increase, reflecting the growing concern associated with leaving it open.

Likewise, increasing the home’s Watchfulness may immediately increase a checkpoint’s Brightness even though the underlying sensor state has not changed.

Brightness is therefore more than a simple indication of whether a condition exists—it communicates **how significant that condition currently is**.

Observers use this continuously changing assessment when determining whether a response should occur.

Because Brightness is published as the state of an Indigo device, homeowners may also use it in their own Indigo triggers, conditions, and Action Groups, making it a powerful semantic indicator throughout their automation system.

![[SecurifyLogo200.png]]