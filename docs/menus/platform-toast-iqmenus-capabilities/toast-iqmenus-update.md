---
title: Updating existing menu entities
excerpt: >-
  Toast IQ can update specific fields on each menu entity type. The fields it
  can change are listed per entity below. Anything not listed must be updated in
  Menu Manager or Edit…
hidden: false
metadata:
  description: >-
    Toast IQ can update specific fields on each menu entity type. The fields it
    can change are listed per entity below. Anything not listed must be updated
    in Menu Manager or Edit…
---

Toast IQ can update specific fields on each menu entity type. The fields it can change are listed per entity below. Anything not listed must be updated in Menu Manager or Edit Menus.

### Update a menu

Editable fields on a menu:

- Course (prep sequence)
- Prep stations
- Assembly line

Preparation settings on a menu are set directly.

### Update a menu group

Editable fields on a menu group:

- Inherit prep sequence (on/off) and a specific prep sequence when not inheriting
- Inherit prep stations (on/off) and specific prep stations when not inheriting
- Inherit assembly line (on/off) and a specific assembly line when not inheriting

Editing a menu group's name, visibility, or pricing is not supported through Toast IQ.

### Update a menu item

Editable fields on a menu item:

- Name
- Description (marketing description)
- Base price
- Image path
- Prep time (in seconds)
- Order in ticket
- Inherit prep sequence (on/off) and a specific prep sequence when not inheriting
- Inherit prep stations (on/off) and specific prep stations when not inheriting
- Inherit assembly line (on/off) and a specific assembly line when not inheriting

A menu item must have a non-empty name. Toast IQ will refuse a request that would set a blank name for a menu item, because items with empty names are not orderable on the POS.

Examples:

- "Rename the Margherita Pizza to Margherita."
- "Set the prep time on the Quesadilla to 5 minutes."
- "Move the Caesar Salad to print first on the kitchen ticket."

### Update a modifier group

Editable fields on a modifier group:

- Name
- Required (yes/no)
- Selection rules: minimum selections, maximum selections, multi-select, and whether the same modifier can be selected more than once
- Pricing strategy
- Pricing mode (e.g. adjusts price, included, fixed price)
- POS short name

Examples:

- "Make the Salad Dressing modifier group required."
- "Allow customers to pick up to 3 toppings on the Pizza Toppings modifier group."

### Update a modifier

Editable fields on a modifier:

- Name
- Base price

> ❗️ Important
>
> Toast IQ can fully update a modifier's price only when the modifier uses the base (default) pricing strategy. For modifiers with menu-specific or time-specific pricing, Toast IQ updates the base price but explicitly notes that the menu- or time-specific prices are unchanged. For size, open, location-specific, or price level pricing, Toast IQ updates the base price but warns the change will not take effect under the active pricing strategy. If the parent modifier group is set to *Included* (no charge) or to a fixed group price, Toast IQ explains that the modifier-level price update may have no effect and offers to update the modifier group price instead.

Examples:

- "Rename the Hot Sauce modifier to Xolula and set its price to $0.75."
- "Increase the price of every modifier in the Breakfast Sides modifier group by 10%."
