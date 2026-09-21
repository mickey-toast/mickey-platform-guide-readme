---
title: Verify automated item firing and prep times
excerpt: >-
  If you enter prep times for your menu items, the Toast platform uses them to
  time when items are fired to the KDS. In order for the prep times to be used,
  however, you must…
hidden: false
metadata:
  description: >-
    If you enter prep times for your menu items, the Toast platform uses them to
    time when items are fired to the KDS. In order for the prep times to be
    used, however, you must…
---

If you enter prep times for your menu items, the Toast platform uses them to time when items are fired to the KDS. In order for the prep times to be used, however, you must enable the [item fire by prep time](https://doc.toasttab.com/doc/platformguide/adminFireByPrepTime.html#adminItemFireByPrepTime) feature.

To verify that this feature is enabled for your restaurant, you must have the **Web Setup > Kitchen / Dining Room Setup** access permission. Then, follow these steps.

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).
2. Choose **Kitchen > Pacing > Meal pacing** to open the **Meal pacing** page.
3. In the **Item Pacing** section, review the setting of the **Item Fire by Prep Time** option. Check the **Enable item fire by prep time** box if necessary.
4. Save and publish your changes.

   After you enable item fire by prep time, the Toast platform uses prep times to schedule and fire items in all orders that appear on KDS devices. The system fires menu items that do not have prep times immediately.

You can also use **Menus > Menu management > Advanced properties** to review the prep times on file for all menu items and modifiers. For more information, see [Configuring prep times for menu items](https://doc.toasttab.com/doc/platformguide/adminFireByPrepTime.html#adminConfigurePrepTimesItems) or [Configuring prep times for integral modifiers](https://doc.toasttab.com/doc/platformguide/adminFireByPrepTime.html#adminConfigurePrepTimesModifiers).
