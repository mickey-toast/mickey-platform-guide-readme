---
title: Creating an item routing rule
excerpt: 'Toast IQ can create a new item routing rule. Editable fields include:'
hidden: false
metadata:
  description: 'Toast IQ can create a new item routing rule. Editable fields include:'
---

Toast IQ can create a new item routing rule. Editable fields include:

- Name
- Condition: exactly one of dining option or service area
- The prep station you reroute from
- The prep station or stations you reroute to

> ❗️ Important
>
> An item routing rule must specify exactly one condition: either a dining option *or* a service area, never both. Rule names do not need to be unique; if you create a rule with a duplicate name, Toast IQ flags the duplicate during confirmation so you can rename it.

Example queries:

- "Add an item routing rule that sends takeout orders from the Grill to the Expo station."
- "Reroute Patio service area items from the Bar to the Cocktail and Expo stations."
