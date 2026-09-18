---
title: Minimum modifiers and visibility settings
excerpt: >-
  When you configure a modifier group to require guests and servers to choose a
  minimum number of modifiers from that group, you must also pay careful
  attention to the ordering…
hidden: false
metadata:
  description: >-
    When you configure a modifier group to require guests and servers to choose
    a minimum number of modifiers from that group, you must also pay careful
    attention to the ordering…
---

When you configure a modifier group to require guests and servers to choose a minimum number of modifiers from that group, you must also pay careful attention to the [ordering channel visibility](https://doc.toasttab.com/doc/platformguide/adminVisibilitySettings.html) settings for the modifiers in that group. Specifically, you must ensure that the number of modifiers that are visible in any given ordering channel meet or exceed the minimum number of modifiers a guest or server must select from the modifier group.

For example, consider a Lunch Sides modifier group that requires guests and servers to pick a minimum of 2 modifiers from it. This Lunch Sides group has the following modifiers:

- Fries
- Salad
- Soup

The Fries modifier is visible on both the Toast POS app and the Toast Online Ordering site but the Soup and Salad modifiers were mistakenly configured so that they are only visible on the Toast POS app. When a guest on the Toast Online Ordering site places an order, they will only see the Fries modifier in the Lunch Sides modifier group, making it impossible for them to pick two sides. The guest will still be allowed to place this order and the order will not fail when it is sent to the Toast platform, but it will not have all the information the kitchen needs to fulfill it.
