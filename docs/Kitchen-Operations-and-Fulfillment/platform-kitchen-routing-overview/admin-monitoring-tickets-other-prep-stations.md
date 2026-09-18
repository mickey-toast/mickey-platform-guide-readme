---
title: Monitoring items at other prep stations
excerpt: >-
  In some restaurants, employees at one prep station need to be aware when other
  prep stations are involved in fulfilling items in the same order. For example,
  a kitchen that…
hidden: false
metadata:
  description: >-
    In some restaurants, employees at one prep station need to be aware when
    other prep stations are involved in fulfilling items in the same order. For
    example, a kitchen that…
---

In some restaurants, employees at one prep station need to be aware when other prep stations are involved in fulfilling items in the same order. For example, a kitchen that does not have an [*expediter*](doc:admin-glossary#glossExpediter) relies on employees at a particular prep station to coordinate order fulfillment or on close communication among employees to synchronize order fulfillment. Including information about other involved prep stations on the ticket can help ensure effective cooperation.

The Toast platform allows you to configure kitchen tickets to display other prep stations working on an item or order on both KDS and printed tickets. For KDS tickets, all prep stations monitor each other automatically. For printed tickets, you [must specify which other prep stations a prep station will monitor](https://doc.toasttab.com/doc/platformguide/adminMonitoringTicketsOtherPrepStations.html#adminKitchenMonitorPrintedTickets).

> 📘 Note
>
> You must have the **6. Web Setup > 6.2 Kitchen / Dining Room Setup** permission to configure a prep station to monitor another prep station.

Some things to keep in mind when using this feature:

- Individual item tickets do not show prep stations for other items in the order; they only show other prep stations for the one item.

   For example, an item sent to a single prep station will not show other prep stations. If an item is sent to multiple prep stations, those prep stations are indicated on the KDS or printed ticket.
- Prep station monitoring only applies to items within the same course. For example, you have items in an *Appetizers* course, and items in an *Entrees* course. Prep stations assigned to the *Entrees* course items will not show on the *Appetizers* course ticket and vice versa: they only show for the items in the course. For more information about courses, see [Assigning courses](https://doc.toasttab.com/doc/platformguide/adminAssigningCourses.html).
- If items in an order only go to a single prep station, they are not shown or printed at other prep stations.

   For example, if all items in an order go to one prep station, there is no need to show the items at another prep station.

**To configure showing other stations working on a ticket**

> 📘 Note
>
> This setting must be configured to enable other station monitoring for both KDS and printed kitchen tickets.

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).
2. Choose **Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup**.
3. Under the Printed Tickets and Ticket Screens section, navigate to the **Other stations** setting.
4. Select the **For each ticket, list other stations working on that ticket** option.
5. Save and publish.

### Monitoring KDS tickets

For KDS tickets, the other prep stations working on items in the order are included automatically at the bottom of the ticket when configured to show other stations.

In the following example, employees at all prep stations need to know when an item or order includes work at other prep stations. This is done automatically when printed and screen tickets are configured to show other stations.

![The Other Stations setting is configured to show other prep stations working on the same ticket. Both "Cold" and "Hot" prep station tickets show what other prep station is working on the order using ALSO AT, followed by the prep station name.](https://doc.toasttab.com/doc/media/kds-other-stations-ticket-diagram.png)

The ticket for the Cold prep station shows the Cold prep station item (Cobb Salad), and includes **ALSO AT: HOT** at the bottom of the ticket to reference the Hot prep station item (Crab Cakes). The ticket for the Hot prep station shows the Hot prep station item (Crab Cakes) and includes **ALSO AT: COLD** at the bottom of the ticket to reference the Cold prep station item (Cobb Salad).

> 📘 Note
>
> If you have the limited release **Send to** setting for prep stations, prep stations set to **Expediter only** are not listed with other prep stations working on the KDS ticket.

### Monitoring printed kitchen tickets

For printed kitchen tickets, you specify which other prep station(s) you want to monitor at a given prep station. When an order includes items that are routed to both prep stations, kitchen tickets print the name of the monitored prep station and a list of menu items routed to that prep station at the end of the ticket. For more information about configuring other stations for printed tickets, see [To configure a prep station to monitor another prep station](https://doc.toasttab.com/doc/platformguide/adminMonitoringTicketsOtherPrepStations.html#adminConfigurePrintOtherStationsItems).

In the following example, employees at the Cold prep station need to know when an order includes menu items routed to the Hot prep station. The employees at the Hot prep station do not need information about menu items at other stations, so they see only the menu items they are responsible for fulfilling. The Cold prep station is configured to have “Hot” as the **Other station**.

![The Cold prep station is configured with the Hot prep station as its other station. When a guest orders both a cold and a hot item, the ticket at the Cold prep station shows the involvement of the Hot prep station, but the ticket at the Hot prep station only shows the hot item.](https://doc.toasttab.com/doc/media/prep_other_station_ex_1.png)

The ticket for the Cold prep station shows the Cold prep station item (Cobb Salad) first followed by the Hot prep station item (Crab Cakes). The ticket for the Hot prep station shows only the Hot prep station item.

If the employees at the Hot prep station do need to monitor the participation of another station, you can configure the Hot prep station to have the Cold prep station as the **Other station**.

![The Cold prep station is configured with the Hot prep station as its other station and vice versa. When a guest orders both a cold and a hot item, the ticket at the Cold prep station shows the involvement of the Hot prep station, and the ticket at the Hot prep station shows the involvement of the Cold prep station.](https://doc.toasttab.com/doc/media/prep_other_station_ex_2.png)

The ticket for the Cold prep station shows the Cold prep station item (Cobb Salad) first, followed by the Hot prep station item (Crab Cakes). The ticket for the Hot prep station shows the Hot prep station item first, followed by the Cold prep station item.

When an order includes menu items from a single prep station, a ticket only prints for that prep station.

![A guest orders a cold item and a hot item, the Cold prep station is configured with the Hot prep station as its other station, so the ticket at the Cold prep station shows both items but the ticket at the Hot prep station only shows the hot item.](https://doc.toasttab.com/doc/media/prep_other_station_ex_3.png)

The ticket for the Hot prep station shows only the Hot prep station item. Nothing is sent to the Cold prep station.

You must have the **6. Web Setup > 6.2 Kitchen / Dining Room Setup** permission to configure a prep station to monitor another prep station.

> 📘 Note
>
> The **Prep stations** page has recently changed. To see how to monitor other prep stations on the legacy page, see the [legacy **Prep stations** page procedure](https://doc.toasttab.com/doc/platformguide/adminMonitoringTicketsOtherPrepStations.html#adminConfigurePrintOtherStationsItemsLegacy).

**To configure a prep station to monitor another prep station**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).
2. Go to **Kitchen > Kitchen stations > Prep stations**. The **Prep stations** page opens.

   ![An example of the Prep stations configuration page in Toast Web.](https://doc.toasttab.com/doc/media/platform-kitchen-prep-station-pg.png)
3. Open the **Edit prep station** pane. To do this, you can either:

   - Select the name of the prep station.
   - Select the overflow menu (the ⋮ icon), and select **Edit prep station** from the content menu.
4. In the **Other stations** section, use the **Select prep stations** dropdown menu to select other prep stations to include on printed tickets. When items assigned to that additional prep station are included in the same order, they are also printed on the ticket under a separate prep station heading.
5. Select **Save**.
6. Publish your changes when ready.

   > 📘 Note
   >
   > Toast Support recommends publishing or scheduling publishing changes outside operating hours to avoid confusing employees with unexpected configuration changes.

**To configure a prep station to monitor another prep station using the legacy **Prep stations** page**

> 📘 Note
>
> The **Prep stations** page has recently changed. To see how to monitor other prep stations on the new page, see the [**Prep stations** page procedure](https://doc.toasttab.com/doc/platformguide/adminMonitoringTicketsOtherPrepStations.html#adminConfigurePrintOtherStationsItems).

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).
2. Go to **Kitchen > Kitchen stations > Prep stations**.

   ![An example of the legacy Prep stations configuration page in Toast Web.](https://doc.toasttab.com/doc/media/platform-kitchen-prep-station-pg-legacy.png)
3. Go to the prep station that should monitor another prep station.
4. Under the **Other Stations** column, select the prep station to monitor.

   ![The Prep Stations page, with the Other Stations column emphasized.](https://doc.toasttab.com/doc/media/print_other_prep_station.png)
5. Save and publish your changes.

For more information about working with prep stations, see [Adding a prep station](https://doc.toasttab.com/doc/platformguide/adminAddPrepStation.html).
