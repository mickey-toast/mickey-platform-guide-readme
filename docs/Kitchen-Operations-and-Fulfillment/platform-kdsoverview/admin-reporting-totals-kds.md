---
title: Reporting item or ingredient totals with the KDS
excerpt: >-
  Keeping track of how many items or ingredients should be in progress, across
  all fired items, is an important tactic for efficiency and waste reduction.
  Mentally tracking…
hidden: false
metadata:
  description: >-
    Keeping track of how many items or ingredients should be in progress, across
    all fired items, is an important tactic for efficiency and waste reduction.
    Mentally tracking…
---

Keeping track of how many items or ingredients should be in progress, across all fired items, is an important tactic for efficiency and waste reduction. Mentally tracking totals, however, can be difficult to do accurately in a fast-paced, high-volume kitchen. With Toast POS devices, you can use either, or both, of these features to report continuously updated totals for fired items or ingredients on the KDS device.

- All day view, which reports a total for each unique menu item, with or without totals for modifiers.
- Production items, which report totals for specific ingredients. You configure production items independently of menu items so that you can track ingredients that are used in multiple menu items and modifiers.

These features count only fired items, and do not report items that are in sent or scheduled status.

In addition, this [Toast Support article](https://support.toasttab.com/article/KDS-All-Day-1493055871075) provides an overview of all day view, and this [Toast Support article](https://support.toasttab.com/article/Production-Item-Count) provides an overview of production items.

### About all day view

When you [enable all day view](https://doc.toasttab.com/doc/platformguide/adminReportingTotalsKDS.html#adminEnableAllDayView) for your restaurant, an **All Day View** option appears in the KDS device title bar. Employees can use this feature to see totals for identical menu items, with or without information about modifiers, by temporarily switching from the ticket screen to all day view. All day view gives your kitchen employees a way to verify how many of each item they need to be working on at any given time.

An example of the KDS device for a sports bar that specializes in chicken wings and chicken tenders served with different kinds of sauces follows.

![A KDS device showing 13 tickets for chicken wings, chicken tenders, and chicken lettuce wraps. The All Day View option in the title bar is circled.](https://doc.toasttab.com/doc/media/KDS_ticket_view_all_day_circled.png)

To see the current total for each unique menu item with a fired item, select **All Day View**. In the following illustration, all day view is configured to show item names and totals only.

![A KDS device's All Day View screen showing total counts for three different menu items.](https://doc.toasttab.com/doc/media/KDS_all_day_items.png)

Kitchen employees might prefer this configuration of all day view if a server or packer is responsible for adding separate modifiers to each menu item right before serving.

Another configuration option for all day view adds the course (if any) and the totals for modifiers under each menu item.

![A KDS device's All Day View screen showing total counts for the same three menu items, with the selected modifiers shown under each one.](https://doc.toasttab.com/doc/media/KDS_all_day_mods.png)

Kitchen employees might prefer this configuration of all day view if the menu items need to be made using the selected modifiers, instead of being added right before serving.

To return to the ticket view from all day view, select **All Day View**.

> 📘 Note
>
> For legacy KDS view, the **All Day View** option appears as **Show All Day View** when all day view is not shown and **Hide All Day View** when shown.

### Update all day view

By default, all day view is enabled for all restaurants to display item names and totals. To update your configuration of all day view, you must have the **Web Setup > Kitchen / Dining Room Setup** access permission. Then, follow these steps.

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).
2. Go to **Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup** to open the **Kitchen** page.
3. In the **Ticket Screens** section, select one of these settings for **All Day Display**.

   - To show a total across tickets for each menu item that currently appears on the KDS device, select **Yes, enable All Day Display, grouped by item only**.
   - To show the course and a subtotal for each variation introduced by modifiers under each menu item total, select **Yes, enable All Day Display, grouped by item and sub-grouped by modifiers**.
   - To remove the **Show All Day View** option from the KDS device ticket view, select **No, do not enable All Day Display**.
4. Save and publish your changes.
