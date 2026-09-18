---
title: >-
  Customizing menu items included in a menu group for a location or location
  group
excerpt: >-
  If you use a menu group across multiple locations, but need to change the menu
  items included in the menu group at specific locations or groups, you can do
  so using overrides.…
hidden: false
metadata:
  description: >-
    If you use a menu group across multiple locations, but need to change the
    menu items included in the menu group at specific locations or groups, you
    can do so using overrides.…
---

If you use a menu group across multiple locations, but need to change the menu items included in the menu group at specific locations or groups, you can do so using overrides. For example, a menu group applies to the Corporate group. The menu items in this menu group are used by all locations in this group, unless you use overrides. For more information, see [Overrides](https://doc.toasttab.com/doc/platformguide/platformOverrides.html).

> 📘 Note
>
> [Required items](https://doc.toasttab.com/doc/platformguide/platformOverridesRequiringMenuItemsInMenuGroup.html) cannot be removed and are indicated with a red asterisk.

### Creating a custom item list for a location or location group

To create an override for the menu items in a menu group, you need permission to edit menu group items for the location or group that the menu group applies to. For example, you want to add an override to the menu group Breakfast, which applies to the Corporate group. To add an override for a Baltimore location, you need edit permissions for the Corporate group.

**To create a custom item list for a menu group**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/index.html).
2. Go to **Menus > Menu management > Menu manager**. The **Menu manager** page opens.
3. From the **Show** section, choose **Full menu**.
4. Select the locations whose menu data you want to edit from the [locations control](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingSearchAndFilteringToFindMenuEntities.html#platformMenuManagerFilteringByLocation).
5. Use the [expand icons](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingAndCustomizingTheMenuManagerViews.html#platformMenuManagerExpandingAndCollapsingRows) to locate the menu group you want to edit.
6. Select the name of the menu group. A side pane opens.
7. In the **Items** section, select **Item lists by location**.

   ![The Items lists by location section of a menu group with no custom item lists.](https://doc.toasttab.com/doc/media/mlx-overrides-item-lists-by-location-new.png)
8. Select **+ Add custom item list**. The **Add custom item list** dialog opens.

   ![The Add custom item list dialog.](https://doc.toasttab.com/doc/media/mlx-overrides-add-custom-item-list-dialog.png)
9. Select the **Applies to** dropdown menu. The **Select location** dialog opens.
10. Select the location or group for the custom item list. The **Select location** dialog closes. The **Add custom item list** dialog now displays the items included by default.

   ![The Add custom item list dialog, showing the items in the list.](https://doc.toasttab.com/doc/media/mlx-overrides-add-custom-item-list-dialog-w-items.png)

   > 📘 Note
   >
   > You can only create one custom item list for each location or group.
11. Edit the items included in the custom item list:

   - Use the remove icon to delete items from the list.

      > 📘 Note
      >
      > [Required items](https://doc.toasttab.com/doc/platformguide/platformOverridesRequiringMenuItemsInMenuGroup.html) cannot be removed.
   - Use **+ Add existing** to search for existing items by menu item name. Select the items you want to add.
   - Change the order of the items using the reorder icon.
12. Select **Create item list**. The dialog closes. A new entry is added under **Item lists by location**.

   ![The Items lists by location section of a menu group with the new custom item list.](https://doc.toasttab.com/doc/media/mlx-overrides-item-lists-by-location-existing.png)
13. At the bottom of the side pane, select **Save**.
14. [Publish your changes when ready](https://doc.toasttab.com/doc/platformguide/publishingChangesForMultipleLocations.html).

### Editing a custom item list for a location or location group

After you create a custom item list, you can edit its items by selecting the pencil icon.

**To edit an existing custom item list for a menu group**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/index.html).
2. Go to **Menus > Menu management > Menu manager**. The **Menu manager** page opens.
3. From the **Show** section, choose **Full menu**.
4. Select the locations whose menu data you want to edit from the [locations control](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingSearchAndFilteringToFindMenuEntities.html#platformMenuManagerFilteringByLocation).
5. Use the [expand icons](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingAndCustomizingTheMenuManagerViews.html#platformMenuManagerExpandingAndCollapsingRows) to locate the menu group you want to edit.
6. Select the name of the menu group. A side pane opens.
7. In the **Items** section, select **Item lists by location**.

   ![The Items lists by location section of a menu group with an existing custom item list.](https://doc.toasttab.com/doc/media/mlx-overrides-item-lists-by-location-existing.png)
8. To edit a custom item list, select the pencil icon on the right side of the row. The **Edit custom item list** dialog opens.

   ![The Edit custom item list dialog, showing the items in the list.](https://doc.toasttab.com/doc/media/mlx-overrides-edit-custom-item-list-dialog.png)
9. Edit the items included in the custom item list:

   - Use the remove icon to delete items from the list.

      > 📘 Note
      >
      > [Required items](https://doc.toasttab.com/doc/platformguide/platformOverridesRequiringMenuItemsInMenuGroup.html) cannot be removed.
   - Use **+ Add existing** to search for existing items by menu item name. Select the items you want to add.
   - Change the order of the items using the reorder icon.
10. Select **Submit**. The dialog closes. The entry under **Item lists by location** is updated.

   ![The Items lists by location section of a menu group with the updated custom item list.](https://doc.toasttab.com/doc/media/mlx-overrides-item-lists-by-location-updated.png)
11. At the bottom of the side pane, select **Save**.
12. [Publish your changes when ready](https://doc.toasttab.com/doc/platformguide/publishingChangesForMultipleLocations.html).

### Deleting a custom item list for a location or location group

To delete a custom item list, select the delete icon (trash can) to the right of a custom item list row. When you delete a custom item list, a confirmation message appears asking you to confirm the deletion. This confirmation message specifies the values the location or location group will use after the custom item list is deleted. Select **Delete** to confirm.

![An example of the deletion confirmation dialog for a custom item list.](https://doc.toasttab.com/doc/media/mlx-overrides-delete-custom.png)

For example, a default list applies to the East location group, which includes Baltimore and Philadelphia. If you delete the custom item list that applies to Baltimore, the Baltimore location will now use the same values as the East location group.
