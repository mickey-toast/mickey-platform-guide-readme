---
title: Saving changes to multiple versions of a menu item
excerpt: >-
  The multi-location menu builder pages allow you to save changes to multiple
  versions of a menu item. For example, you can save pricing updates to one or
  more versions of a menu…
hidden: false
metadata:
  description: >-
    The multi-location menu builder pages allow you to save changes to multiple
    versions of a menu item. For example, you can save pricing updates to one or
    more versions of a menu…
---

> 📘 Note
>
> This feature is in [limited release](https://doc.toasttab.com/doc/platformguide/techReleaseNotesLimitedRelease.html).

The multi-location menu builder pages allow you to save changes to multiple versions of a menu item. For example, you can save pricing updates to one or more versions of a menu item, instead of viewing and updating each version separately.

You start by viewing the details page for one version of the menu item. This is your *current version*. You make your changes to the current version and then select the **Save to multiple** button. This opens a two-step dialog that lets you select:

- The changes you want to apply to the other versions. You can choose to apply all the changes or just some of them.
- The additional versions you want to apply the changes to. You can apply the changes to all the other versions or just some of them.

When you select **Save**, the current and additional versions are updated according to your selections.

****Important note about settings with multiple values****

Settings that can have more than one value, for example, prep stations and tax rates, are not supported in the save to multiple versions dialog. If you make changes on the menu item page for a setting with this limitation, and then go to the dialog, you see the setting in the changes list. A banner below the list indicates you cannot apply the setting's changes to other versions. When you select **Save** in the dialog, the setting's changes are applied *to the current version only*.

![Example of the save to multiple versions dialog, showing the banner for a setting with multiple values.](https://doc.toasttab.com/doc/media/menu-builder-mlm-save-to-multiple.png)

**To save changes to multiple versions of a menu item**

1. Log in to [Toast Web](https://doc.toasttab.com/doc/platformguide/adminToastPosAccessTypes.html).
2. Go to **Menus > Bulk management > Advanced Properties**.
3. From the **You are viewing** menu, pick a location group that uses a menu that contains the item you want to edit and select **Update**.
4. Expand the menu and locate the menu item, then select its name to open its classic details page.
5. In the banner at the top of the classic page, select the `new item page` link. The menu builder page for the menu item opens.

   ![Location of the menus experience link.](https://doc.toasttab.com/doc/media/menu-builder-mlm-new-item-page-link.png)
6. Edit the menu item's settings.
7. Select the down arrow next to the **Save** button, and then select **Save to multiple versions**.
8. Select the changes you want to apply to other versions, and then select the versions you want to apply those changes to.
9. Select **Save**. You return to the menu item's page with a notification that your item has been updated across multiple versions.
10. Publish your changes using the **Toast account > Publishing > Publish config** page. For more information, see [Publishing changes for multiple locations](https://doc.toasttab.com/doc/platformguide/publishingChangesForMultipleLocations.html).
