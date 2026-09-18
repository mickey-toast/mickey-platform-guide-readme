---
title: Overrides
excerpt: >-
  If you use an entity across multiple locations, but need a specific setting to
  differ at certain locations, you can use overrides. Overrides differ from
  versions in that they…
hidden: false
metadata:
  description: >-
    If you use an entity across multiple locations, but need a specific setting
    to differ at certain locations, you can use overrides. Overrides differ from
    versions in that they…
---

If you use an entity across multiple locations, but need a specific setting to differ at certain locations, you can use *overrides*. Overrides differ from [versions](https://doc.toasttab.com/doc/platformguide/versions.html) in that they provide setting-level differences, while keeping the rest of the entity the same. Overrides also allow differences between locations to be maintained in a single entity, compared to versions, where you maintain a separate entity for each location.

> 📘 Note
>
> Toast Support recommends using either overrides or versions, but never both.

For example, you have two locations: Ann Arbor and Baltimore. A sandwich menu item is the same at both locations except that at Baltimore, the sandwich menu item uses an additional Grill prep station. In this example, both locations use a single version of the sandwich menu item, and you create a custom prep stations list for the Baltimore location that adds the Grill prep station.

> 📘 Note
>
> You can only create one override for each location or location group.

### Prerequisites for creating overrides

Before you create an override for a specific location, you need permission to edit that setting at the location or group-level that the entity applies to. For example, a menu item applies to the Corporate group. To add a custom prep time to the menu item for the Baltimore location, which is part of the Corporate group, you need permission to edit the menu item at the Corporate group-level.

### Understanding defaults

For each setting that has overrides available, there is a default. The default includes the values applied to the same location or group the entity applies to. Any overrides are variations of this default.

For example, the sandwich item applied to the Corporate group has the Corporate group level settings as the default. If you add an override for the Baltimore location, the Baltimore location uses the override, while all other locations in the group use the default. If the Baltimore override is deleted, the Baltimore location returns to using the Corporate group settings.

For more information about location hierarchy, see [Restaurant groups and sub-groups](https://doc.toasttab.com/doc/platformguide/restaurantGroupsAndSubgroups.html).

### Override settings

Currently, the overrides feature is only available for the following settings:

- [Menu items included in a menu group](https://doc.toasttab.com/doc/platformguide/platformOverridesCustomMenuItemListInMenuGroup.html)
- [Prep time of a menu item](https://doc.toasttab.com/doc/platformguide/platformOverridesCustomPrepTimeForMenuItem.html)
- [Prep stations assigned to a menu item](https://doc.toasttab.com/doc/platformguide/platformOverridesCustomPrepStationsForMenuItem.html)
