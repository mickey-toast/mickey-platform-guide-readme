---
title: Creating menu entities
excerpt: >-
  Toast IQ can create new menus, menu groups, menu items, modifier groups, and
  modifiers. The fields it accepts at creation time are listed per entity below.
  Anything not listed…
hidden: false
metadata:
  description: >-
    Toast IQ can create new menus, menu groups, menu items, modifier groups, and
    modifiers. The fields it accepts at creation time are listed per entity
    below. Anything not listed…
---

Toast IQ can create new menus, menu groups, menu items, modifier groups, and modifiers. The fields it accepts at creation time are listed per entity below. Anything not listed must be configured in Toast Web after Toast IQ creates the entity.

### Create a menu

Toast IQ can create one or more new menus in a single request. Editable fields:

- Menu name

Examples:

- "Create a Brunch menu."
- "Create three menus called Breakfast, Lunch, and Dinner."

### Create a menu group

Toast IQ can create one or more menu groups. A menu group can be added either directly under a menu or nested as a subgroup under another menu group — Toast IQ asks which when it isn't clear from your request. Editable fields:

- Menu group name
- Parent menu or parent menu group

Examples:

- "Add a new Sides menu group under the Dinner menu."
- "Create a Subs subgroup inside the Sandwiches menu group."

### Create a menu item

Toast IQ can create one or more menu items at a time. Each new item is added to a specific menu group that you name in the request. Editable fields:

- Name
- Base price
- Description
- Parent menu group

> ❗️ Important
>
> Toast IQ creates menu items with the base (default) pricing strategy and a price set on the item itself. Items that need open pricing, size-based pricing, menu-specific pricing, time-specific pricing, location-specific pricing, or price levels must be created or have their pricing strategy set in [Menu builder overview](https://doc.toasttab.com/doc/platformguide/adminMenuBuilderOverview.html) or [Items database overview](https://doc.toasttab.com/doc/platformguide/platformItemsDatabaseOverview.html).

Examples:

- "Create a Caesar Salad menu item in the Salads group for $12."
- "Add Espresso, Latte, and Cappuccino to the Coffee menu group, $4 each."

### Create a modifier group

Toast IQ can create a modifier group, populate it with brand-new or existing modifiers, and optionally attach it to one or more menu items or menu groups in the same request. Toast IQ requires at least one modifier when creating a modifier group, because empty modifier groups make their parent items un-orderable on the POS and online ordering. Editable fields:

- Name
- Whether the modifier group is required or optional
- Selection rules: minimum selections, maximum selections, multi-select, and whether the same modifier can be selected more than once
- Pricing strategy and pricing mode (including a fixed group price)
- POS short name
- Initial modifiers — either existing modifiers (by name) or brand new ones with a name and base price
- Optional parents — menu items and menu groups to attach the new modifier group to

Examples:

- "Create a Salad Dressing modifier group on the Caesar Salad with Ranch, Italian, and Balsamic options."
- "Add a Cheese Add-Ons modifier group to all of the burger items, with Cheddar, Swiss, and American at $1 each."

### Create a modifier

Toast IQ can create a standalone modifier or create one and attach it to an existing modifier group. Editable fields:

- Name
- Base price (omit for a free modifier)
- Optional modifier group to attach to

> ❗️ Important
>
> Toast IQ creates modifiers with the base (default) pricing strategy and individual (per-modifier) pricing. It does not create modifiers with size, sequence, or other advanced pricing strategies. If the parent modifier group enforces a single shared price, Toast IQ asks whether to drop the per-modifier price or switch the group to individual pricing.

Examples:

- "Add Rainbow Sprinkles to the Toppings modifier group for 50 cents extra."
- "Add Bacon to the Burger Add-Ons group for $2.50."
