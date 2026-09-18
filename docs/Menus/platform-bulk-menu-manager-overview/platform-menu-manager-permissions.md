---
title: Menu manager permissions
excerpt: 'The menu manager is controlled by these permissions:'
hidden: false
metadata:
  description: 'The menu manager is controlled by these permissions:'
---

The menu manager is controlled by these permissions:

- **4. Restaurant Admin > 4.5 Edit Full Menu**
- **4. Restaurant Admin > 4.14 Local Menu Edit**
- **6. Web Setup > 6.4 Publishing**
- **6. Web Setup > 6.7 Change sets**

The following sections provide more details.

### Permissions for accessing menu manager

You must have the **4. Restaurant Admin > 4.5 Edit Full Menu** or the **4. Restaurant Admin > 4.14 Local Menu Edit** permission to the location you are logged into to access the menu manager. If you do not have one of these permissions, you will not see the **Menus > Menu management > Menu manager** option in Toast Web.

### Permissions for editing menus

To make edits to your menus, you must have the permissions described in the sections below.

#### For single location restaurants

Employees with the **4. Restaurant Admin > 4.5 Edit Full Menu** permission can edit any aspect of the menu, using any of the [menu manager views: Full menu, Items, Modifiers, or Price levels](https://doc.toasttab.com/doc/platformguide/platformMenuManagerViewingOptions.html).

Employees with the **4. Restaurant Admin > 4.14 Local Menu Edit** permission cannot see the **Full menu** view and are limited to the following menu edits in the other views:

- Menu item prices, using the **Items** view. For more information, see [Editing a menu item's price](https://doc.toasttab.com/doc/platformguide/platformMenuManagerWorkingWithMenuItems.html#platformMenuManagerEditingAMenuItemsPrice).
- Modifier prices, using the **Modifiers** view. For more information, see [Specifying modifier prices](https://doc.toasttab.com/doc/platformguide/platformWorkingWithModifiersMenuManager.html#platformSpecifyingModifiersPricesMenuManager).
- Prices for price levels, using the **Price levels** view. For more information, see [Editing a price level's price](https://doc.toasttab.com/doc/platformguide/platformMenuManagerWorkingWithPriceLevels.html#platformMenuManagerEditingAPriceLevelsPrice).

For employees with the **Local Menu Edit** permission, the other menu entity properties are grayed out to indicate you cannot edit them.

#### For multi-location restaurants

To edit a menu entity, you must have the **4. Restaurant Admin > 4.5 Edit Full Menu** or **4. Restaurant Admin > 4.14 Local Menu Edit** permission to that menu entity's [owner](https://doc.toasttab.com/doc/platformguide/ownersAndPermissions.html), or to one of the owner's parents in the location group hierarchy.

For example, consider the following location group hierarchy:

- Corporate

   - Northeast Franchises

      - Boston
      - New York City

And the following menu items and their owners:

- Pasta Primavera, Owner: Corporate
- Turkey Club, Owner: Northeast Franchises
- Lobster, Owner: Boston

If you have the **Edit Full Menu** or **Local Menu Edit** permission to the:

- Corporate group, you can edit all three menu items because all three menu items are owned by the Corporate group or a child of the Corporate group.
- Northeast Franchises group, you can edit the Turkey Club, which is owned by the Northeast Franchises group, and the Lobster, which is owned by Boston, a child of the Northeast Franchises group.
- Boston location, you can only edit the Lobster menu item.

The type of edits you are allowed to make depend on the permission you have. Employees with the **Edit Full Menu** permission can edit any aspect of the menu entity, using any of the [menu manager views: Full menu, Items, Modifiers, or Price levels](https://doc.toasttab.com/doc/platformguide/platformMenuManagerViewingOptions.html).

Employees with the **Local Menu Edit** permission cannot see the **Full menu** view and are limited to the following menu edits in the other views:

- Menu item prices, using the **Items** view. For more information, see [Editing a menu item's price](https://doc.toasttab.com/doc/platformguide/platformMenuManagerWorkingWithMenuItems.html#platformMenuManagerEditingAMenuItemsPrice).
- Modifier prices, using the **Modifiers** view. For more information, see [Specifying modifier prices](https://doc.toasttab.com/doc/platformguide/platformWorkingWithModifiersMenuManager.html#platformSpecifyingModifiersPricesMenuManager).
- Prices for price levels, using the **Price levels** view. For more information, see [Editing a price level's price](https://doc.toasttab.com/doc/platformguide/platformMenuManagerWorkingWithPriceLevels.html#platformMenuManagerEditingAPriceLevelsPrice).
- For menu items and modifiers that use location-specific prices, you can edit the prices for locations where you have **Local menu edit** access, even if the entity is owned by a location group you don't have **Local menu edit** access to.

For employees with the **Local Menu Edit** permission, the other menu entity properties are grayed out and cannot be edited.

If you *do not* have the **Edit Full Menu** or **Local Menu Edit** permission to a menu entity's [owner](https://doc.toasttab.com/doc/platformguide/ownersAndPermissions.html), or to one of the owner's parents in the location group hierarchy, but that entity is used by one of your locations, then the menu manager does the following:

- In the **Items**, **Modifiers**, and **Price levels** views, the menu entity is visible so you can see its configuration, but you cannot edit it.
- In the **Full menu** view, the menu entity is visible in the menu hierarchy table but the user interface controls that allow you to edit it, for example, the reorder icon and the overflow menu, are hidden.

   When you select the entity, the side pane opens so you can see its configuration, but a banner at the top of the pane indicates that the information is read-only.

If you *do not* have the **Edit Full Menu** or **Local Menu Edit** permission to a menu item's owner, or to one of the owner's parents in the location group hierarchy, but that menu item has location-specific prices that are used by your locations, then you can see the menu item in **Items** view and edit the prices that are used by your locations. The same is true of modifier item references: you can see and edit location-specific prices on modifiers that are used by your locations in **Modifiers** view.

For more information, see [Owners and permissions](https://doc.toasttab.com/doc/platformguide/ownersAndPermissions.html).

### Permissions for publishing changes

To make menu configuration changes available to the Toast API and Toast platform, you must publish them after you save them. For example, you add a new item to a menu or change menu prices. When you save those changes, they are not reflected on Toast POS devices or in Toast API results until you publish them. If you manage multiple locations, you must make sure that you publish changes to all of the locations where the changes apply.

On the Toast platform, you have two options for publishing your changes. You can publish the changes manually when you are ready for employees and guests to see them or you can schedule them to be published at a specific date and time in the future. The [Permissions for manual publishing](https://doc.toasttab.com/doc/platformguide/platformMenuManagerPermissions.html#platformMenuManagerPermissionsForManualPublishing) and [Permissions for scheduled publishing](https://doc.toasttab.com/doc/platformguide/platformMenuManagerPermissions.html#platformMenuManagerPermissionsForScheduledPublishing) sections below describe the permissions you need for manual publishing and scheduled publishing.

If you don't have the correct publishing permissions, you can still save your changes but you cannot publish them, either manually or using scheduled publishing.

> 📘 Note
>
> Changes you make on **Full menu** view must be manually published because this view does not support scheduled publishing. The **Items**, **Modifiers**, and **Price levels** views support both manual and scheduled publishing.

> 📘 Note
>
> For information on deciding when you should publish your changes, see [Understanding when to publish your menu](https://doc.toasttab.com/doc/platformguide/adminUnderstandingWhenToPublishYourMenuMenuManager.html). For information on using the two publishing workflows, see [Publishing menu manager changes](https://doc.toasttab.com/doc/platformguide/platformPublishingMenuManagerChanges.html).

#### Permissions for manual publishing

To manually publish changes you make in menu manager, you must have the **6. Web Setup > 6.4 Publishing** permission as described below:

- For single-location restaurants, you must have the **Publishing** permission at the location you are logged into.
- For multi-location restaurants, you must have the **Publishing** permission to the locations you are publishing changes for.

#### Permissions for scheduled publishing

The scheduled publishing feature, which is available on the **Items**, **Modifiers**, and **Price levels** views, lets you make changes to your Toast configuration that are then saved and published at a later date and time. When you use this feature, you create change sets. A change set records updates you want to make to your Toast platform configuration. At the date and time you specify, the updates in the change set are saved to the [saved database](https://doc.toasttab.com/doc/platformguide/platformUnderstandingSavingAndPublishing.html) and then immediately published to the [published database](https://doc.toasttab.com/doc/platformguide/platformUnderstandingSavingAndPublishing.html), making them available to employees and guests.

The scheduled publishing feature requires both the **6. Web Setup > 6.7 Change sets** and **6. Web Setup > 6.4 Publishing** permissions, as described below.

- To add changes to a new change set, you need the **6. Web Setup > 6.4 Publishing** and **6. Web Setup > 6.7 Change sets** permissions to the location you are logged into.
- To add changes to an existing change set, you need the **Publishing** and **Change sets** permissions to the location or location group (or an ancestor of the location or location group) specified in the change set's **Editable by** setting.
- You can view a list of active change sets by selecting the **View scheduled** button to open the **Which change sets would you like to view?** dialog. Change sets in this dialog are limited to those where you have the **Change sets** permissions to the location or location group (or an ancestor of the location or location group) specified in the change set's **Editable by** setting.

   The illustration below shows the location of the **View scheduled** button.

   ![The location of the View scheduled button.](https://doc.toasttab.com/doc/media/menu-manager-view-scheduled-button.png)

   The illustration below shows an example of the **Which change set would you like to view?** dialog.

   ![Example of the Which change sets would you like to view? dialog.](https://doc.toasttab.com/doc/media/menu-manager-which-change-sets-to-view.png)
- The menu manager displays a [change set icon](https://doc.toasttab.com/doc/platformguide/platformColumnsInTheMenuManagerViews.html#platformMenuManagerItemAndModifierColumns_ChangeSetIndicator) next to menu entities that are affected by change sets. Selecting this icon displays a list of change sets you have access to that affect this entity.

   The change sets in this list are limited to change sets where you have the **Change sets** permission to the location or location group (or an ancestor of the location or location group) specified in the change set's **Editable by** setting.

   It is possible that there are change sets that affect a menu entity to which *you do not have access*. These change sets are not visible in the list of change sets you see when selecting a change set icon. Also, the icon itself is only shown if there are change sets *you have access to* that affect the menu entity. If you do not have access to any of the change sets that affect a menu entity, no change set icon appears for it.

   ![The location of the calendar icon for a menu item.](https://doc.toasttab.com/doc/media/menu-manager-changeset-indicator.png)

It is important to note that the **Change sets** and **Publishing** permissions only give you permission to work with the change sets themselves. To edit the changes *stored* in a change set, you must have additional permissions specific to the type of changes you want to store. In the case of menu manager, you must have the **4. Restaurant Admin > 4.5 Edit Full Menu** or **4. Restaurant Admin > 4.14 Local Menu Edit** permission as described in [Permissions for editing menus](https://doc.toasttab.com/doc/platformguide/platformMenuManagerPermissions.html#platformMenuManagerMenuEditingPermissions).

> 📘 Note
>
> For more information about saving and publishing, including the difference between them, see [Understanding saving and publishing](https://doc.toasttab.com/doc/platformguide/platformUnderstandingSavingAndPublishing.html). For more information about change sets, see [Understanding scheduled publishing and change sets](https://doc.toasttab.com/doc/platformguide/platformUnderstandingScheduledPublishingAndChangeSets.html).
