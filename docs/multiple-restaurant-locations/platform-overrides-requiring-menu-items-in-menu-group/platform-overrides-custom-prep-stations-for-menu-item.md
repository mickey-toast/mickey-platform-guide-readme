---
title: Customizing prep stations assigned to an item for a location or location group
excerpt: >-
  If you use a menu item across multiple locations, but need to change the prep
  stations assigned to the item at specific locations, you can create an
  override for the prep…
hidden: false
metadata:
  description: >-
    If you use a menu item across multiple locations, but need to change the
    prep stations assigned to the item at specific locations, you can create an
    override for the prep…
---

If you use a menu item across multiple locations, but need to change the prep stations assigned to the item at specific locations, you can create an override for the prep stations. For example, a menu item applies to the Corporate group. All locations in the group use these prep stations, unless you use an override. For more information, see [Overrides](https://doc.toasttab.com/doc/platformguide/platformOverrides.html).

> 📘 Note
>
> If you inherit prep stations from the menu group or menu, you cannot create overrides.

### Creating custom prep stations

To create an override for the prep stations assigned to a menu item, you need permission to edit an item’s assigned prep stations for the location or group that the menu item applies to. For example, you want to add an override to the Sandwich menu item, which applies to the Corporate group. To add an override for a Baltimore location, you need edit permissions for the Corporate group.

**To create custom prep stations**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/index.html).
2. Go to **Menus > Menu management > Menu manager**. The **Menu manager** page opens.
3. From the **Show** section, choose **Full menu**.
4. Select the locations whose menu data you want to edit from the [locations control](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingSearchAndFilteringToFindMenuEntities.html#platformMenuManagerFilteringByLocation).
5. Use the [expand icons](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingAndCustomizingTheMenuManagerViews.html#platformMenuManagerExpandingAndCollapsingRows) to locate the menu item you want to edit.
6. Select the name of the menu item. A side pane opens.
7. In the **Kitchen** section, go to the **Prep stations** setting.

   ![The Prep stations setting of a menu item with no custom prep stations.](https://doc.toasttab.com/doc/media/mlx-overrides-prep-stations-no-custom.png)
8. Depending on whether custom prep stations have already been created, you can either:

   - Select the **+** icon.
   - Under the **Customize by location** table, select **+ Add custom prep stations**.

   The **Add custom prep stations** dialog opens.

   ![The Add custom prep stations dialog.](https://doc.toasttab.com/doc/media/mlx-overrides-add-custom-prep-stations-dialog.png)
9. Select the **Applies to** dropdown menu. The **Select location** dialog opens.
10. Select the location or group for the custom prep stations. The **Select location** dialog closes. The **Add custom prep stations** dialog now displays the prep stations assigned by default.

   ![The Add custom prep stations dialog with the prep stations assigned.](https://doc.toasttab.com/doc/media/mlx-overrides-add-custom-prep-stations-dialog-w-prep-stations.png)

   > 📘 Note
   >
   > You can only create one custom prep stations list for each location or group.
11. Edit the prep stations included in the custom prep stations list:

   - To add a prep station, select the **Prep stations** dropdown menu, and choose the prep stations you want to use. You can use the search bar to find a specific prep station.
   - To remove all prep stations currently assigned, select **Clear all**.
   - To remove a single prep station, you can either:

      - Below the **Prep stations** dropdown menu, select the button with the prep station name followed by an X.
      - Clear the checkbox of a prep station in the **Prep stations** dropdown menu.
12. Select **Submit**. The **Add custom prep stations** dialog closes. A new entry is added to the **Customize by location** table.

   ![The Prep stations setting of a menu item with a new custom prep station list.](https://doc.toasttab.com/doc/media/mlx-overrides-prep-stations-existing.png)
13. At the bottom of the side pane, select **Save**.
14. [Publish your changes when ready](https://doc.toasttab.com/doc/platformguide/publishingChangesForMultipleLocations.html).

### Editing custom prep stations

After you create a custom prep stations list, you can edit its prep stations by selecting the pencil icon.

> 📘 Note
>
> You cannot change which location or location group the custom prep stations apply to. You can only change which prep stations are included in the list.

**To edit custom prep stations**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/index.html).
2. Go to **Menus > Menu management > Menu manager**. The **Menu manager** page opens.
3. From the **Show** section, choose **Full menu**.
4. Select the locations whose menu data you want to edit from the [locations control](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingSearchAndFilteringToFindMenuEntities.html#platformMenuManagerFilteringByLocation).
5. Use the [expand icons](https://doc.toasttab.com/doc/platformguide/platformMenuManagerUsingAndCustomizingTheMenuManagerViews.html#platformMenuManagerExpandingAndCollapsingRows) to locate the menu item you want to edit.
6. Select the name of the menu item. A side pane opens.
7. In the **Kitchen** section, go to the **Prep stations** setting.

   ![The Prep stations setting of a menu item with an existing custom prep stations list.](https://doc.toasttab.com/doc/media/mlx-overrides-prep-stations-existing.png)

   > 📘 Note
   >
   > Optionally, use the **Filter by group/location** dropdown menu to help find a specific custom prep station list.
8. To edit a custom prep stations list, select the pencil icon on the right side of the row. The **Edit custom prep stations** dialog opens.

   ![The Edit custom prep stations dialog with the prep stations assigned.](https://doc.toasttab.com/doc/media/mlx-overrides-edit-custom-prep-stations-dialog.png)
9. Edit the prep stations included in the custom prep stations list:

   - To add a prep station, select the **Prep stations** dropdown menu, and choose the prep stations you want to use. You can use the search bar to find a specific prep station.
   - To remove all prep stations currently assigned, select **Clear all**.
   - To remove a single prep station, you can either:

      - Below the **Prep stations** dropdown menu, select the button with the prep station name followed by an X.
      - Clear the checkbox of a prep station in the **Prep stations** dropdown menu.
10. Select **Submit**. The **Edit custom prep stations** dialog closes. The **Customize by location** table entry is updated with your changes.

   ![The Prep stations setting of a menu item with an updated custom prep stations list.](https://doc.toasttab.com/doc/media/mlx-overrides-prep-stations-updated.png)
11. At the bottom of the side pane, select **Save**.
12. [Publish your changes when ready](https://doc.toasttab.com/doc/platformguide/publishingChangesForMultipleLocations.html).

### Deleting custom prep stations

You can delete custom prep stations using the delete icon (trash can) to the right of a custom prep stations row. When you delete custom prep stations, a confirmation message appears asking you to confirm the deletion. This confirmation message specifies the values the location or location group will use after the custom prep stations are deleted. Select **Delete** to confirm.

![An example of the deletion confirmation dialog for custom prep stations.](https://doc.toasttab.com/doc/media/mlx-overrides-delete-custom.png)

For example, default prep stations apply to the East location group, which includes Baltimore and Philadelphia. If you delete the custom prep stations that apply to Baltimore, the Baltimore location will now use the same prep stations as the East location group.
