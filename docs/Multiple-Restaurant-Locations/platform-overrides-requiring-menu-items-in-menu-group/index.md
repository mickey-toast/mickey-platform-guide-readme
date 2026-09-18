---
title: Requiring a menu item in a menu group at all locations
excerpt: >-
  When an item is marked as required, the location or location group assigned to
  the menu group automatically includes the required item. Required items cannot
  be removed when…
hidden: false
metadata:
  description: >-
    When an item is marked as required, the location or location group assigned
    to the menu group automatically includes the required item. Required items
    cannot be removed when…
---

> 📘 Note
>
> To mark items as required, you must have the [**Edit Full Menu**](https://doc.toasttab.com/doc/platformguide/adminPermissions.html#permissionEditFullMenu) permission for the location or location group the menu group applies to.

When an item is marked as required, the location or location group assigned to the menu group automatically includes the required item. Required items cannot be removed when [creating](https://doc.toasttab.com/doc/platformguide/platformOverridesCustomMenuItemListInMenuGroup.html#platformOverridesCustomMenuItemListInMenuGroupCreate) or [editing a custom item list](https://doc.toasttab.com/doc/platformguide/platformOverridesCustomMenuItemListInMenuGroup.html#platformOverridesCustomMenuItemListInMenuGroupEdit).

Here is an example of the **All items** table, before an item is required. The **Used by** column shows how many locations are currently using this menu item.

![A menu item that is not required and is currently only used by one location.](https://doc.toasttab.com/doc/media/mlx-overrides-before-item-required.png)

Here is an example of the **All items** table after an item is marked as required. The **Used by** column reflects that all locations now use the menu item. You cannot use the remove icon while the menu item is required.

![A menu item that is required and is used by all locations that use this menu group.](https://doc.toasttab.com/doc/media/mlx-overrides-after-item-required.png)

Here is an example of how a required item appears when adding or editing a custom item list. The item is marked by a red asterisk and you can no longer remove the item.

![The required menu item in a custom item list indicating the asterisk and the grayed out remove icon.](https://doc.toasttab.com/doc/media/mlx-overrides-required-items-creating-overrides.png)

**To require items at multiple locations**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/index.html).
2. Go to **Menus > Menu management > Menu manager**. The **Menu manager** page opens.
3. From the **Show** section, choose **Full menu**.
4. Select the locations whose menu data you want to edit from the [locations control](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingSearchAndFilteringToFindMenuEntities.html#platformMenuManagerFilteringByLocation).
5. Use the [expand icons](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingAndCustomizingTheMenuManagerViews.html#platformMenuManagerExpandingAndCollapsingRows) to locate the menu group you want to edit.
6. Select the name of the menu group. A side pane opens.
7. In the **Items** section, select **All items**.
8. Next to the item you want required across all locations, select the **Required** toggle button. The **Used by** column now reflects that the item is used by all possible locations.
9. At the bottom of the side pane, select **Save**.
10. [Publish your changes when ready](https://doc.toasttab.com/doc/platformguide/publishingChangesForMultipleLocations.html).
