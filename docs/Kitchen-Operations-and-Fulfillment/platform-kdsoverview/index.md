---
title: Kitchen display system overview
excerpt: >-
  The kitchen display system (KDS) allows you to use screens instead of printed
  tickets to route and display orders in the kitchen. Using KDS devices allows
  for better…
hidden: false
metadata:
  description: >-
    The kitchen display system (KDS) allows you to use screens instead of
    printed tickets to route and display orders in the kitchen. Using KDS
    devices allows for better…
---

The kitchen display system (KDS) allows you to use screens instead of printed tickets to route and display orders in the kitchen. Using KDS devices allows for better communication between back of house and front of house when the food is ready for guests, and transparency on which parts of an order are completed. If changes are made on Toast POS devices in the front of house, those changes appear on KDS devices in the kitchen in real time. KDS devices also provide visual and auditory settings to inform kitchen employees about order details. These settings include:

- Sound notifications when there is a new ticket, a ticket is ready to be fulfilled at the expediter KDS device, an item is changed, and an item is voided.
- Different ticket heading colors based on the age of the ticket.
- A flash animation to indicate a ticket is new or was changed.

KDS devices are used in the kitchen as either an expediter or prep station KDS device. An expediter device serves as the intermediary place between the front of house and back of house to inform the front of house that an order is ready. A prep station device displays items to prepare at specific preparation areas. You can configure your restaurant to use both expediter and prep station KDS devices, or only expediter or prep station KDS devices.

The following diagram shows how an order might be routed to different KDS devices for a restaurant that uses expediter and prep station KDS devices.

![A diagram showing an example workflow of how an order and items can be routed at a restaurant using expediter and prep station KDS devices.](https://doc.toasttab.com/doc/media/kds-overview-expo-ps-workflow-ex.png)

For this example, fired items are sent to both the expediter KDS device and the appropriate prep station KDS devices. When all items are marked as fulfilled at the prep station, the ticket turns green on the expediter KDS device, indicating that all items are ready. Once the items are physically at the expediter station, the ticket is marked as fulfilled. If you have notifications configured to appear when tickets are fulfilled, the Toast POS device that placed the order initially receives a notification. In this case, the prep stations are configured to [send items and tickets to both prep stations and expediter stations](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configSendTo), and the kitchen uses a [single-level expediter](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configTwoLevelFulfillment). You can also configure a prep station to not send fulfilled items and tickets to the expediter. For example, the Bar prep station is not in the kitchen, so it does not need to send fulfilled items to the expediter KDS device located in the kitchen.

The following diagram shows how an order might be routed to different KDS devices for a restaurant that uses only expediter KDS devices.

![A diagram showing an example workflow of how an order and items can be routed at a restaurant using only expediter KDs devices.](https://doc.toasttab.com/doc/media/kds-overview-expo-only-workflow-ex.png)

For this example, fired items are sent to the expediter KDS device. When individual items are marked as fulfilled on the expediter KDS screen, a green check appears next to the item. Once all items on a ticket are marked as fulfilled, the ticket disappears. If you have notifications configured to appear when tickets are fulfilled, the Toast POS device that placed the order initially receives a notification.

You can choose to use two-level expediter fulfillment and enable whether tickets must be at one expediter before the next one with that two-level expediter fulfillment. For example, to be marked as ready, the ticket needs to be fulfilled at the first expediter before being marked as fulfilled at the second expediter.

The following diagram shows how an order might be routed to different KDS devices for a restaurant that uses only prep station KDS devices.

![A diagram showing an example workflow of how an order and items can be routed at a restaurant using only prep station KDS devices.](https://doc.toasttab.com/doc/media/kds-overview-ps-only-workflow-ex.png)

For this example, fired items are sent to the appropriate prep station KDS devices. When individual items are marked as fulfilled on the prep station screen, a green check appears next to the item. Once all items on a ticket are marked as fulfilled, the ticket disappears. If the prep station is configured to [not send items and tickets to the expediter](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configSendTo) and you have notifications configured to appear when tickets are fulfilled, the Toast POS device that placed the order initially receives a notification.

You can also choose to send items to multiple prep stations. For more information, see [Multiple prep stations for an item](https://doc.toasttab.com/doc/platformguide/adminRoutingToPrepStations.html#platformKitchenMultiplePrepStationAssignment).

### KDS device interface

Here is an example of the expediter KDS device interface, with multiple tickets.

> 📘 Note
>
> Though the KDS device functions differently as either an expediter or prep station, the screen layout remains the same.

![Example of an expediter KDS device with tickets.](https://doc.toasttab.com/doc/media/example-kds-device-screen.png)

At the top-left of the screen, the arrow icon returns you to the Toast home page. On the top-right, there are options to show the [all day view](https://doc.toasttab.com/doc/platformguide/adminReportingTotalsKDS.html#adminAllDayView), show [recently fulfilled tickets](https://doc.toasttab.com/doc/platformguide/adminRedisplayingTickets.html), and [recalling the last fulfilled ticket](https://doc.toasttab.com/doc/platformguide/adminRedisplayingTickets.html#adminRecallTicket). If there is not enough space at the top to display these options, they can appear in the overflow menu. The overflow menu, represented by three vertically stacked dots, provides additional actions and shortcuts.

- **Language**: This option opens a dialog that allows you to change the language of the KDS user interface.
- **Switch to Legacy View**: This option changes the KDS from using new KDS view to legacy KDS view.

   > 📘 Note
   >
   > If you are using legacy KDS view, there is a **Try New KDS (Grid View)** option that changes the KDS device from legacy KDS view to new KDS view.
- **KDS appearance**: This option opens the **KDS appearance** pane for new KDS view, which allows you to choose the ticket layout, text size, and display theme. For more information, see [KDS appearance pane](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKdsAppearancePane).
- **Device Setup**: This option opens the **Device Setup** screen on a POS device. This option is not limited to KDS mode.
- **Switch user**: This option opens the passcode screen, allowing a new employee to enter a passcode and open the Toast POS app. This option is not limited to KDS mode.
- **Device Status**: This option opens a dialog that displays device information, including status for connectivity and services. This option is not limited to KDS mode.

The middle of the screen is the area where tickets display. Tickets appear at the top left and move downward and to the right. If a ticket is longer than the screen, the ticket continues to the next column. Ticket size is not standard, and changes to fit the number of items on the ticket. If the amount of tickets exceeds the screen size, you can swipe right and left on the screen to see tickets beyond the current view.

At the bottom of the screen, there are production items, if configured. For more information about production items, see [About production items](https://doc.toasttab.com/doc/platformguide/adminAssignPrepStationKDS.html#adminAboutProdItems).

### New KDS view

> 📘 Note
>
> Grid view for KDS will now be referred to as the new KDS view. Dynamic view for KDS will now be referred to as legacy KDS view.

New KDS view is the next iteration of Toast's kitchen display system, with a new design and features that set it apart from legacy KDS view:

- [KDS appearance pane](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKdsAppearancePane): Provides a way to choose and personalize the layout, select a text size, and choose a display theme from the overflow menu (the ⋮ icon) on the KDS device.
- [Layout options](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKitchenKdsLayoutOptions): Provides a new grid layout option for kitchen tickets, which sets a maximum number of tickets on a screen in a grid pattern. You can also use the dynamic layout, which is what is used with legacy KDS view. Dynamic layout changes the size of to fit the number of items, allowing you to see as many tickets as possible.
- [Preview tickets](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformGridKDSPreviewTickets): Provides kitchen employees a preview of upcoming tickets as items are added to an order.
- [Navigation](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKitchenKdsNavigation): Includes buttons to go to the first and last tickets on the KDS device and indicates how many tickets are on the KDS device.
- [Payment status](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformGridKDSPaymentStatus): Displays whether the order was paid or unpaid.
- [Dark mode](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformGridKDSDarkMode): A color scheme for the screen that is more optimal for low light or prolonged screen use.
- [Assembly lines](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformGridKDSAssemblyLines): Creates a sequence of prep stations for an item.
- [Load balancing](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKdsLoadBalancing): Divides prep station tickets between multiple prep station KDS devices with the same prep station assigned.
- [Partial fulfillment indicator](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformGridKDSPartialFulfillmentIndicator): A yellow dot icon indicating that the item is being worked on by at least one prep station.
- [Food runner fulfillment](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKitchenKDSFoodRunnerFulfillment): Individual items can be marked as fulfilled on expediter KDS devices. If already fulfilled at the previous level (prep station KDS devices for one expediter and the first level expediter for two-level fulfillment), it shows a single check mark. When fulfilled at the current expediter level (second level expediter for two-level fulfillment) fulfillment of an item on an expediter ticket uses a double check mark.

   > 📘 Note
   >
   > Fulfillment at the previous level is not required to show the double check mark.
- [Viewing recipes](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKitchenKDSViewRecipes): Adds a recipe to a menu item that can be viewed on KDS devices.

   > 📘 Note
   >
   > This feature is in limited release.

> ❗️ Important
>
> New KDS view is only compatible with the local data synchronization method. This local sync method allows for offline mode using local sync. For more information on how local sync works, see [Offline mode with local sync](https://doc.toasttab.com/doc/platformguide/platformOfflineModeLocalSync.html).

Here is an example of the new KDS view on an expediter KDS device:

![An example of an expediter KDS device with two fired tickets and one preview ticket.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-kds-expo-2-fired-1-preview-tickets.png)

At the top-left of the screen, the arrow icon returns you to the Toast POS home screen. On the other side, there are options to show [all day view](https://doc.toasttab.com/doc/platformguide/adminReportingTotalsKDS.html#adminAllDayView), [recently fulfilled tickets](https://doc.toasttab.com/doc/platformguide/adminRedisplayingTickets.html), and to [recall the last fulfilled ticket](https://doc.toasttab.com/doc/platformguide/adminRedisplayingTickets.html#adminRecallTicket). These options may be included in the overflow menu, depending on the screen size of your KDS device.

The overflow menu (the ⋮ icon) options includes:

- **Language**: Opens the **KDS language** dialog. This dialog allows you to change the language used in the user interface for KDS mode.
- **KDS appearance**: Opens the **KDS appearance** pane, which allows you to choose the ticket layout, text size, and display theme. For more information, see [KDS appearance pane](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKdsAppearancePane).
- **Device Setup**: Opens the **Device Setup** page.
- **Switch user**: Opens the POS passcode screen.
- **Device Status**: Opens a dialog showing the device connection and service statuses.

The middle of the screen is the ticket area.

The bottom of the screen is for navigation. For more information, see [Navigation](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKitchenKdsNavigation).

> 📘 Note
>
> The Android navigation bar is hidden on new KDS view to maximize screen space. Swipe upward from the bottom of the screen to reveal it.

#### KDS appearance pane

You can use the **KDS appearance** pane to change the appearance of your KDS device without leaving the screen. On the **KDS appearance** pane, you can:

- Choose the ticket layout.
- Choose the maximum number of rows of tickets on a screen. This is only available if you choose the grid layout.
- Choose the maximum number of columns of tickets on a screen.
- Choose the text size used by the tickets.
- Choose the display theme.

   > 📘 Note
   >
   > This changes the display theme for the device, not just KDS mode.

**To customize the appearance of your KDS device**

1. From the **Kitchen Display System** screen, select the overflow menu (the ⋮ icon) on the top right and select **KDS appearance**. The **KDS appearance** pane opens.

   ![An example of the KDS appearance pane on a KDS device.](https://doc.toasttab.com/doc/media/kitchen-kds-appearance-pane.png)
2. Choose a **Ticket layout**:

   - **Dynamic**: This uses dynamically-sized tickets that change according to the number of items on the ticket.
   - **Grid**: This uses a set number of spaces that are used for tickets. Longer tickets can include multiple spaces.
3. If you selected **Grid**, choose the number of **Rows**. This sets the number of rows of tickets you see on the KDS device.

   The number of rows you can choose from depends on the size of your device.

   > 📘 Note
   >
   > The **Rows** option is only available for the **Grid** ticket layout.
4. Choose the number of **Columns**. This sets the number of columns of tickets you see on the KDS device when the device is in landscape orientation.

   > 📘 Note
   >
   > When the device is in portrait orientation, the number of columns determines the number of rows. For example, if you set **Columns** to **3**, in landscape orientation you have three columns and in portrait orientation you have three rows. Changing the **Rows** setting has no effect while in portrait orientation.

   The number of columns you can choose from depends on the size of your device.
5. Choose a **Text size**. This sets the text size used by KDS tickets.

   You can choose **Small**, **Medium**, **Large**, or **Extra large**.
6. Choose a **Display theme**. This sets the colors used by the user interface.

   This can be **Light mode** or **Dark mode**. For more information, see [Dark mode](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformGridKDSDarkMode).
7. Select **Save**. Your changes are saved and the appearance of your KDS device screen updates to reflect your choices.

#### Changing the KDS view

> 📘 Note
>
> Legacy KDS view will be deprecated. New Toast customer accounts are automatically configured to use new KDS view.

When you initially set up your KDS device, you can choose legacy KDS view (**Legacy View**) or new KDS view (**New Grid View**). This sets the default kitchen view for your Toast POS device. You can change the view by using the **Try New KDS (Grid View)** option at the top of the legacy KDS view screen and selecting the **Try New KDS (Grid View)** button from the dialog, or from the **Device Setup** screen.

> 📘 Note
>
> When you switch from legacy KDS view to new KDS view using the **Device Setup** screen, you are prompted to select the ticket sizing.

**To change the KDS view using the Device Setup screen**

1. Go to the **Device Setup** screen. You can either:

   - From the Toast POS home screen, navigate to the **Setup** section and select **Device Setup**.
   - From the Kitchen Display System mode screen, select the overflow menu (the ⋮ icon) on the top right and select **Device Setup**.

   The **Device Setup** screen opens.
2. Select **KDS View**.
3. Choose **Legacy View** or **New Grid View**.
4. Select **Save**. The **Device Setup** screen appears.

#### Layout options

There are two layout options for new KDS view:

- **Dynamic**: This layout is the classic layout, where the size of tickets adjusts according to the number of items.
- **Grid**: This layout divides the screen into a number of rows and columns, forming a grid. A ticket fills at least one of the grid spaces, and combines with additional spaces depending on the number of items on the ticket.

> 📘 Note
>
> The layout options for new KDS view are configured at the device-level. For example, if you want two KDS devices to use a different layout, you need to configure each device. To change the layout, use the [KDS appearance pane](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKdsAppearancePane).

When using the grid layout, the first ticket fills the top-left grid space and the next ticket fills the grid space below it. Once that grid column is filled, tickets continue to be added to the next column and move downward. Here is an example of the path tickets added to the grid layout take:

![A diagram illustrating the path tickets take when being created using the grid layout. This path moves top to bottom, and fills each column from left to right.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-layout-ticket-path.png)

For tickets that take up more than a single grid space, the ticket expands to the grid space below it. If it continues past that grid space, it continues until the column is filled and then continues to the top grid space of the next column and moves downwards.

Here is an example of a ticket that fills a single grid space.

![An example of a ticket that fits a single grid space on an expediter KDS device.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-layout-one-space-ticket.png)

Here is an example of a ticket that fills two grid spaces.

![An example of a ticket that fits two grid spaces.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-layout-two-space-ticket.png)

For both grid and dynamic layouts, if a ticket is larger than a single column, the ticket breaks and continues to the next column. The ticket at the end of the first column and the beginning of the next column uses a **CONTINUED** label to indicate it is part of the same ticket. If there is a ticket at the top of the column, and the ticket after it does not fit in the remaining space, it moves to the next column.

Here is an example of a KDS device using grid layout with a ticket that covers two columns.

![An example of a KDS device using grid layout with a ticket that covers two columns.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-layout-two-column-ticket.png)

Here is an example of a KDS device using dynamic layout with a ticket that covers two columns.

![An example of a KDS device using dynamic layout with a ticket that covers two columns.](https://doc.toasttab.com/doc/media/kitchen-kds-dynamic-layout-two-column-ticket.png)

> 📘 Note
>
> For both of these examples, the ticket comes after a shorter ticket, so it is moved to a new column.

##### Deprecated ticket behavior

If a ticket is added that is larger than the remaining grid spaces on a screen with tickets, the new ticket is moved to the next page.

Here is an example of a KDS device using the grid layout with three tickets. The third ticket is larger than the remaining grid spaces and is moved to the next page.

![An example of a ticket on a KDS device using the grid layout that is larger than the remaining space on a page and is moved to the next page.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-kds-expo-3-tickets-2-pages.png)

If a ticket is larger than all the grid spaces on a screen, it is continued on the next page. The first section of the ticket is marked with **CONTINUED** on the bottom right corner of the ticket. The last section of the ticket is marked with **CONTINUED** on the top left corner of the ticket. If there are any middle sections, the ticket is marked with **CONTINUED** on both the bottom right and top left corners of the ticket to indicate it is continued on the next and previous pages.

Here is an example of a ticket that is across three pages.

![An example of a ticket on a KDS device using the grid layout that takes up three pages, with CONTINUED on the beginning or end of the ticket to indicate more items either before and after the current page.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-kds-expo-1-ticket-3-pages.png)

You can change the text size and the number of rows and columns at any time using **[KDS appearance pane](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKdsAppearancePane)**.

#### Preview tickets

Preview tickets (fire on next) allow kitchen staff to see items as they are added to an order by providing a preview ticket. The item appears on the preview ticket after the restaurant employee adds the item to the order and begins to enter the next item.

> 📘 Note
>
> Preview tickets are configured at the restaurant level.

The preview ticket is indicated by a shaded portion below the ticket, the word **Preview** replacing the fire time, and the ticket header fading between light and dark gray repeatedly.

![An example of a KDS ticket, with preview tickets enabled, before and after the order is sent. The ticket displays a shaded portion and Preview on the preview ticket before the order is sent, and no shaded portion and a fire timer on a regular ticket after the order is sent.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-kds-ticket-before-after-sent-to-kitchen.png)

> 📘 Note
>
> You cannot see preview tickets for orders placed online or from a kiosk. The ticket appears on the KDS device after the entire order is finalized and sent to the kitchen.

After the ticket is **Sent**, the **Preview** label and ticket shadow disappear, the fading between light and dark gray stops, and the ticket enters a **Sent** state. The **Preview** label is replaced with the fire timer.

> 📘 Note
>
> Preview tickets cannot be fulfilled.

After an order is sent to the kitchen, subsequent additions to the order do not display as a preview ticket. These items are visible on the KDS device once they are sent to the kitchen. For example, if you add two items to an order, these items show on the preview ticket. Once you send the order to the kitchen and then add another item, the item does not appear on the KDS device until you send the order again.

If a future or scheduled order is placed on a Toast POS device, the order appears as a preview ticket until the fire time is met.

Before configuring KDS devices to display preview tickets, consider that preview tickets show all items as they are added to an order. If you configure your restaurant to not send items or courses to the kitchen, once fired, items that did appear on preview tickets disappear from the KDS tickets. For example:

- If the **Kitchen** > **Pacing** > **Meal pacing** > **Sending Courses** setting is set to **Send courses individually**, after an order is sent, only the courses chosen by an employee at the front of house to send to the kitchen appear, with items belonging to courses not sent disappearing from the KDS device. This can lead to confusion for kitchen employees.
- If **Front of house** > **Order screen setup** > **Individually Hold and Send Items** is enabled, once the initial items are sent to the kitchen, the kitchen tickets only show the fired items. This can lead to confusion for kitchen employees.

If you exit or close the Toast POS app while an order is in progress, the preview ticket remains on the screen until the Toast platform clears any outdated tickets. The preview ticket may remain on your device for up to thirty minutes.

**To configure KDS devices to display preview tickets**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).
2. Choose **Kitchen** > **Printers, tickets, & KDS devices** > **Kitchen and ticket setup** to open the **Kitchen** page.
3. In the **Ticket Screens** section, use the **Preview Tickets** setting to turn the preview tickets feature on or off.
4. Select **Save** and **Publish**.

   > 📘 Note
   >
   > To avoid updating while the restaurant is open, Toast support recommends publishing outside restaurant operating hours.

For an example workflow of a KDS device using preview tickets, see [KDS workflow using new KDS view](https://doc.toasttab.com/doc/platformguide/platformGridKDSWorkflow.html).

#### Navigation

> 📘 Note
>
> The navigation on the new KDS has recently changed to use scrolling. Pagination is deprecated. To see the previous method of navigating using pages, see [Pagination](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformGridKDSPagination).

You scroll between all KDS tickets by swiping right and left. When scrolling, the KDS device automatically adjusts to show the entire column width of tickets. For example, if you swipe and only see half of a column, the screen will adjust to show the entire column.

The new KDS uses two buttons that help you navigate quickly to the first and last KDS tickets, and a display of how many tickets are currently visible on the KDS device.

- The left-facing arrow goes to the first ticket on the KDS device.
- The right-facing arrow goes to the last ticket on the KDS device.
- The ticket count reflects how many tickets are currently displayed on the KDS device.

Here is an example of a KDS device, emphasizing the navigation buttons.

![An example of the new KDS view, emphasizing the navigation buttons to the first and last KDS tickets and the ticket counter.](https://doc.toasttab.com/doc/media/kitchen-kds-navigation-buttons.png)

##### Pagination

> 📘 Note
>
> The navigation on the new KDS has recently changed. Pagination is deprecated. To see the new method of navigating, see [Navigation](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKitchenKdsNavigation).

The new KDS view uses **Next** and **Previous** on the bottom right and left of the KDS screen to navigate to the next and previous pages. You can also swipe right and left to navigate to the next and previous pages.

The page number indicator icon at the bottom center is shaded dark gray to indicate the page currently being viewed. You can select a different page number icon to navigate to that specific page.

Here is an example of a KDS device with multiple pages and pagination.

![An example of the new KDS view with two pages, with the current page icon shaded a dark gray.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-kds-pagination.png)

#### Payment status

New KDS view tickets display a payment status, which indicates whether the order for the ticket is paid or not. The payment status can be:

- **NOT PAID**: The entire amount for the order is not received and processed by the restaurant.
- **PAID**: The entire amount for the order is received and processed by the restaurant.

Here is an example of a ticket before and after it is paid.

![An example of a KDS ticket before and after the order is paid. The ticket displays NOT PAID before the payment, on the left, and PAID after the payment, on the right.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-kds-ticket-before-after-payment.png)

#### Dark mode

> 📘 Note
>
> You can also change the display theme using the **KDS appearance** pane. For more information, see [KDS appearance pane](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKdsAppearancePane).

The new KDS view is available in dark mode. To change to dark mode, select the overflow menu (the ⋮ icon), choose **Device Setup**, and select the **POS Display Theme** setting to choose between the **Light mode** and **Dark mode** options. Select **Save** to implement the theme.

Here is an example of a KDS device using dark mode.

![An example of a KDS device using dark mode.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-kds-dark-mode.png)

#### Assembly lines

An assembly line is a sequence of prep stations that you can assign to menu entities that an item follows in the kitchen. Once an item is sent to the kitchen, it appears on the first prep station in the sequence, and once fulfilled at that prep station, it moves to the second prep station in the sequence. This continues until the sequence is completed.

Assembly lines are ideal for kitchens with items that move in a standard path through kitchen prep stations. For example, a pizza restaurant has a menu for pizza items that all go to the ****Dough****, ****Sauce/Toppings****, and ****Bake**** prep stations in that order. Using an assembly line keeps other prep stations from seeing an item before it is fulfilled at the previous prep station in a sequence. For more information about how assembly lines work, see [Routing using assembly lines](https://doc.toasttab.com/doc/platformguide/platformKDSRoutingUsingAssemblyLines.html). For information about how to create an assembly line, see [Creating an assembly line](https://doc.toasttab.com/doc/platformguide/platformKDSCreatingAssemblyLines.html).

Before you start creating and assigning assembly lines, verify the following:

- You created prep stations.
- You set the [**Fulfillment Method**](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configFulfillmentMethod) setting to **Fulfill at each station independently**.
- You verified that the menu entity and the assembly line you plan to assign to that menu entity use at least one of the same prep stations.

#### Load balancing

Load balancing divides kitchen tickets between multiple prep station KDS devices that are assigned the same prep station. This feature allows tickets to be worked on between the load-balancing groups without tickets appearing multiple times on the prep station KDS devices assigned to the same prep station. A ticket can be claimed for a load-balancing group, and does not appear on prep station KDS devices in another load-balancing group.

For information about how to set up load balancing, see [Configuring load balancing](https://doc.toasttab.com/doc/platformguide/platformKitchenConfiguringLoadBalancing.html). For information about how load balancing works, see [Routing using load balancing](https://doc.toasttab.com/doc/platformguide/platformKitchenRoutingUsingLoadBalancing.html).

#### Partial fulfillment indicator

If you set the [**Fulfillment Method**](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configFulfillmentMethod) setting to **Fulfill at each station independently**, a partial fulfillment indicator appears on expediter KDS tickets for items that have been partially fulfilled.

> 📘 Note
>
> The prep station assigned to an item must [send to prep station and expediter](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configSendTo) in order to start partial fulfillment on the expediter KDS device tickets.

The partial fulfillment indicator appears as a yellow dot to the left of the item name. It indicates that an item was fulfilled by at least one prep station, but not all assigned prep stations. Once the item is fulfilled at all prep stations, the indicator changes to a green check mark, indicating that the item was fulfilled at all prep stations.

Here is an example of a ticket on an expediter KDS device with one item using the partial fulfillment indicator and another item marked as fulfilled at all prep stations.

![An example of a partial-fulfillment indicator and a fulfilled at all prep stations indicator on an expediter KDS device ticket.](https://doc.toasttab.com/doc/media/kds-partial-fulfillment-indicator.png)

#### Food runner fulfillment

> 📘 Note
>
> To use food runner fulfillment, the [**Fulfill Items**](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configFulfillItems) setting must be set to **Enable individual item fulfillment**.

The food runner fulfillment feature allows employees to fulfill individual items on expediter KDS device tickets. Food runner fulfillment is useful in situations where items are given to the guest as soon as they are ready, giving a visual indication of the fulfillment status of an individual item for that KDS device and fulfillment level.

If a ticket with multiple items contains an item that is fulfilled at a prep station KDS device, or at the previous station or stations for expediter KDS devices, it is marked with a green check mark. When an item on a ticket is fulfilled at the highest fulfillment level by an employee, the Toast platform marks the item with a green double check mark on that expediter KDS device.

- If you use [two-level fulfillment](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configTwoLevelFulfillment), the highest level of fulfillment is at the second-level expediter KDS device. The green double check mark appears when the item is fulfilled at the second-level expediter KDS device.
- If you use single-level fulfillment, the highest level of fulfillment is at the expediter KDS device. The green double check mark appears when the item is fulfilled at the expediter KDS device.

Here is an example of two tickets on the expediter KDS device: one with the green check mark, and another with the double check mark.

![Examples of an expediter ticket with an item marked with a green check mark indicating it was fulfilled at the previous station and a green double check mark indicating it was fulfilled at the expediter KDS device.](https://doc.toasttab.com/doc/media/kds-food-runner-fulfillment-icons.png)

Food runner fulfillment only works for expediter KDS device tickets with multiple items. Once a ticket or all of the items on a ticket are fulfilled, the ticket disappears from the KDS device.

#### Viewing recipes

> 📘 Note
>
> This feature is in limited release.

If a menu item has a recipe associated with it and the **[Fulfill Items](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configFulfillItems)** setting is set to **Enable individual item fulfillment**, you can view the recipe on a KDS device.

For information about how to add a recipe to a menu item, see [Adding a recipe view](https://doc.toasttab.com/doc/platformguide/platformMenuManagerWorkingWithMenuItems.html#platformMenuManagerAddingRecipeView).

> 📘 Note
>
> Recipes can only be added to menu items.

**To view a menu item recipe on a KDS device**

1. On the KDS device, select a ticket to open the ticket dialog.

   ![An example of the ticket dialog on a KDS device, emphasizing the recipe icons.](https://doc.toasttab.com/doc/media/kds-ticket-dialog-with-recipe-icon.png)
2. Select one item that has the recipe icon.

   > 📘 Note
   >
   > Selecting more than one item, even if both have recipes, hides the **View Recipe** button.

   ![An example of a single menu item selected in the ticket dialog on a KDS device, with the View Recipe button visible.](https://doc.toasttab.com/doc/media/kds-menu-item-with-recipe-selected.png)
3. Select the **View Recipe** button. The recipe file opens.

   ![An example of a recipe file viewed on a KDS device.](https://doc.toasttab.com/doc/media/kds-viewing-recipe.png)
4. When you are done reading the recipe, select the **Close** button or tap outside of the recipe dialog.

#### New KDS view and legacy KDS view

In addition to new features only on the new KDS view, new KDS view also implements several existing features differently from legacy KDS view to maximize efficiency. These differences apply to:

- Production items
- Ticket header
- Action to fulfill
- Average fulfillment timer

##### Production items

While legacy KDS view supports any number of production items, new KDS view supports a maximum of *30* production items. When viewing a new KDS view device in landscape orientation, 30 production items appear as five rows, with six items in each row. In portrait orientation, 30 production items appear as six rows, with five items in each row.

Here is an example of the new KDS view with eight production items.

![An example of new KDS view with eight production items.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-kds-production-items.png)

For more information about production items, see [About production items](https://doc.toasttab.com/doc/platformguide/adminAssignPrepStationKDS.html#adminAboutProdItems).

##### Ticket header

While legacy KDS view displays the dining option beneath the header, new KDS view has moved the dining option to the header itself.

Here is an example of a ticket on new KDS view, compared to a ticket on legacy KDS view.

![A comparison of a kitchen ticket in both new KDS view and legacy KDS view.](https://doc.toasttab.com/doc/media/kitchen-kds-new-versus-legacy-tickets.png)

##### Action to fulfill

In addition to the double-tap action, you can also swipe downwards anywhere on the ticket itself to either fulfill or unfulfill it for new KDS view. The motion fulfills or unfulfills the ticket depending on whether you have **Double tap to fulfill** or **Double tap to unfulfill** enabled. By default, the setting is **Double tap to fulfill**, meaning swiping downwards or double tapping fulfills the ticket.

##### Average fulfillment timer

While the average fulfillment timers for legacy KDS view are visible on the top left of the KDS device, average fulfillment timers for new KDS view appear on the bottom right and on top of kitchen tickets. On expediter KDS devices, the timer can be collapsed to only show the first expediter timer, or expanded to see all prep stations timers related to the expediter KDS device.

Here is an example of the average fulfillment timers on a prep station KDS device using new KDS view.

![An example of the average fulfillment timer on the bottom right of a prep station KDS device.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-avg-fulfill-timer-prep.png)

Here is an example of the average fulfillment timers on an expediter KDS device using new KDS view with most timers hidden.

![An example of the average fulfillment timer on the bottom right of an expediter KDS device, with timers collapsed.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-avg-fulfill-timer-expo-collapsed.png)

Select **+ Expand Timers** to show all timers related to the expediter KDS device.

Here is an example of an expediter KDS device with all average fulfillment timers visible.

![An example of the average fulfillment timer on the bottom right of an expediter KDS device, with timers expanded.](https://doc.toasttab.com/doc/media/kitchen-kds-grid-avg-fulfill-timer-expo-expanded.png)

If there are more timers that do not fit on the expanded view, you can swipe up and down within the average fulfillment timer dialog to see timers that are not visible.

Select **+ Collapse Timers** to hide all timers except for the expediter timer on the expediter KDS device.

For more information about average fulfillment timers, see [Understanding average fulfillment timers](https://doc.toasttab.com/doc/platformguide/platformKitchenAvgFullfillmentTimer.html).

#### New KDS view usage guidelines

When using new KDS view, use the following guidelines:

- **Do not** use new KDS view on portable devices. New KDS view is not currently compatible with ToastGo1 and ToastGo2 devices. Using new KDS view on these devices can result in cropped contents and poor formatting.
- **Do not** disconnect your local hub device from your router. The local hub device is required for offline mode with local sync. For more information about the local hub device, see [Local hub devices](https://doc.toasttab.com/doc/platformguide/platformOfflineModeLocalSync.html#platformOfflineModeLocalSyncLocalHubDevice).
- **Be aware** that clearing the app data or uninstalling the Toast POS app on a new KDS view device will prompt you to choose settings that configure the appearance of your KDS device.
