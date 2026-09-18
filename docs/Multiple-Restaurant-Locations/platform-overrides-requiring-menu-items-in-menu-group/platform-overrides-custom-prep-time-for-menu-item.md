---
title: Customizing an item’s prep time for a location or location group
excerpt: >-
  If you use a menu item across multiple locations, but need to change the prep
  time for the item at specific locations, you can create an override for the
  prep time. For…
hidden: false
metadata:
  description: >-
    If you use a menu item across multiple locations, but need to change the
    prep time for the item at specific locations, you can create an override for
    the prep time. For…
---

If you use a menu item across multiple locations, but need to change the prep time for the item at specific locations, you can create an override for the prep time. For example, a menu item applies to the Corporate group. All locations in the group use this prep time, unless you use an override. For more information, see [Overrides](https://doc.toasttab.com/doc/platformguide/platformOverrides.html).

### Creating a custom prep time for a location or location group

To create an override for the prep time of a menu item, you need permission to edit an item’s prep time for the location or group that the menu item applies to. For example, you want to add an override to the Sandwich menu item, which applies to the Corporate group. To add an override for a Baltimore location, you need edit permissions for the Corporate group.

**To create a custom prep time**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/index.html).
2. Go to **Menus > Menu management > Menu manager**. The **Menu manager** page opens.
3. From the **Show** section, choose **Full menu**.
4. Select the locations whose menu data you want to edit from the [locations control](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingSearchAndFilteringToFindMenuEntities.html#platformMenuManagerFilteringByLocation).
5. Use the [expand icons](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingAndCustomizingTheMenuManagerViews.html#platformMenuManagerExpandingAndCollapsingRows) to locate the menu item you want to edit.
6. Select the name of the menu item. A side pane opens.
7. In the **Kitchen** section, go to the **Prep time** setting.

   ![The Prep time setting of a menu item with no custom prep times.](https://doc.toasttab.com/doc/media/mlx-overrides-prep-time-setting-no-custom.png)
8. Depending on whether a custom prep time has already been created, you can either:

   - Select the **+** icon to show the **Customize by location** table.
   - Under the **Customize by location** table, select **+ Add custom prep time**.

   A new custom prep time entry appears.

   ![The Prep time setting of a menu item with a new custom prep time entry.](https://doc.toasttab.com/doc/media/mlx-overrides-prep-time-setting-new-custom.png)
9. In the **Seconds** field, enter the number of seconds it takes to prepare the item.
10. Select the dropdown menu under the **Applies to** column. The **Select location** dialog opens.
11. Select the location or group for the custom prep time. The **Select location** dialog closes. The location or group is added to the custom prep time entry.

   ![The Prep time setting of a menu item with a new custom prep time.](https://doc.toasttab.com/doc/media/mlx-overrides-prep-time-setting-new-custom-added.png)

   > 📘 Note
   >
   > You can only create one custom prep time for each location or group.
12. At the bottom of the side pane, select **Save**.
13. [Publish your changes when ready](https://doc.toasttab.com/doc/platformguide/publishingChangesForMultipleLocations.html).

### Editing a custom prep time for a location or location group

Once you create a custom prep time for a location or location group, you can use the **Seconds** field to change the prep time as needed. However, you cannot update which location or group the custom prep time applies to.

**To edit an existing custom prep time**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/index.html).
2. Go to **Menus > Menu management > Menu manager**. The **Menu manager** page opens.
3. From the **Show** section, choose **Full menu**.
4. Select the locations whose menu data you want to edit from the [locations control](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingSearchAndFilteringToFindMenuEntities.html#platformMenuManagerFilteringByLocation).
5. Use the [expand icons](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingAndCustomizingTheMenuManagerViews.html#platformMenuManagerExpandingAndCollapsingRows) to locate the menu item you want to edit.
6. Select the name of the menu item. A side pane opens.
7. In the **Kitchen** section, go to the **Prep time** setting.

   ![The Prep time setting of a menu item with an existing custom prep time.](https://doc.toasttab.com/doc/media/mlx-overrides-prep-time-setting-new-custom-added.png)
8. In the **Seconds** field of the custom prep time you want to change, enter the number of seconds it takes to prepare the item.

   > 📘 Note
   >
   > Optionally, use the **Filter by group/location** dropdown menu to help find a specific custom prep time.

   ![The Prep time setting of a menu item with an updated custom prep time.](https://doc.toasttab.com/doc/media/mlx-overrides-prep-time-setting-updated-custom.png)
9. At the bottom of the side pane, select **Save**.
10. [Publish your changes when ready](https://doc.toasttab.com/doc/platformguide/publishingChangesForMultipleLocations.html).

### Deleting a custom prep time for a location or location group

To delete a custom prep time, select the delete icon (trash can) to the right of a custom prep time row. When you delete a custom prep time, a confirmation message appears asking you to confirm the deletion. This confirmation message specifies the values the location or location group will use after the custom prep time is deleted. Select **Delete** to confirm.

![An example of the deletion confirmation dialog for a custom prep time.](https://doc.toasttab.com/doc/media/mlx-overrides-delete-custom.png)
