---
title: KDS configuration quick reference
excerpt: >-
  The kitchen display system (KDS) offers a number of options for changing the
  way information reaches your employees.
hidden: false
metadata:
  description: >-
    The kitchen display system (KDS) offers a number of options for changing the
    way information reaches your employees.
---

The kitchen display system (KDS) offers a number of options for changing the way information reaches your employees.

This section presents a quick reference guide to the changes you can make to better meet the needs of your back of house employees. A series of tables present options for how the KDS device presents information, how you make a change, whether the setting affects all devices or an individual device, and the [access permissions](https://doc.toasttab.com/doc/platformguide/adminPermissions.html) that you need.

### KDS notification options

You can signal new and changed orders to back of house employees in different ways by setting the options described in the following table.

| If you want to... | Toast Web (All devices) | Toast POS home screen (Each device) | Required Permission |
|---|---|---|---|
| Play a sound when a new ticket appears, a ticket is ready for fulfillment at an expediter KDS devices, an item is changed, and an item is marked as void |  | Setup > Device Setup > New Ticket Sound | Device Setup > 7.3 KDS and Order Screen Setup |
| Flash changed tickets | Kitchen > Printers, tickets, & KDS devices> Kitchen and ticket setup > [Flash Changes](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configFlashChanges): Flash changes |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| Change ticket colors as they age | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [Warning Colors](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configWarningColors): Enabled |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| Print tickets if needed | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [Print On Demand](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configPrintOnDemand): Enable |  | Web Setup > 6.2 Kitchen / Dining Room Setup |

For more information about how to change configuration settings, see [Accessing the Toast POS Device Setup screen](https://doc.toasttab.com/doc/platformguide/adminConfigureDevice.html) or [Using Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).

### KDS interaction options

You define how back of house employees interact with the KDS device to fulfill tickets and view consolidated ([*All Day*](doc:admin-glossary#glossAllDay)) totals by setting the options described in the following table.

| If you want to... | Toast Web (All devices) | Toast POS home screen (Each device) | Required Permission |
|---|---|---|---|
| Fulfill complete tickets | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [Fulfill Items](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configFulfillItems): Disable |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| Fulfill tickets item by item | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [Fulfill Items](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configFulfillItems): Enable |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| Fulfill with a double tap |  | Setup > Device Setup > Double-tap to Fulfill, Unfulfill | Device Setup > 7.3 KDS and Order Screen Setup |
| Fulfill with a tap to select then a tap on **Fulfill** |  | Setup > Device Setup > Double-tap to Fulfill, Unfulfill | Device Setup > 7.3 KDS and Order Screen Setup |
| Unfulfill with a double tap |  | Setup > Device Setup > Double-tap to Fulfill, Unfulfill | Device Setup > 7.3 KDS and Order Screen Setup |
| Unfulfill with a tap to select then a tap on **Unfulfill** |  | Setup > Device Setup > Double-tap to Fulfill, Unfulfill | Device Setup > 7.3 KDS and Order Screen Setup |
| Add the option to see item totals in **All Day Display** | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [All Day Display](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configAllDayDisplay): Yes, enable All Day Display, grouped by item... |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| Add the option to see modifier and item totals in **All Day Display** | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [All Day Display](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configAllDayDisplay): Yes, enable All Day Display, grouped by item and... |  | Web Setup > 6.2 Kitchen / Dining Room Setup |

For more information about how to change configuration settings, see [Accessing the Toast POS Device Setup screen](https://doc.toasttab.com/doc/platformguide/adminConfigureDevice.html) or [Using Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).

### KDS ticket contents

You define what information appears on tickets by setting the options described in the following table.

| If you want to... | Toast Web (All devices) | Toast POS home screen (Each device) | Required Permission |
|---|---|---|---|
| See other prep stations working on ticket items | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [Other Stations](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configOtherStations): For each ticket, list... |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| See all courses fired at once and the status of each course | Kitchen > Pacing > Meal pacing > Course Pacing: Enable course pacing > Sending Courses: Send all courses individually >[Previous Course Status](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configPreviousCourseStatus): Show the status... |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| [Color-code](https://doc.toasttab.com/doc/platformguide/platformKitchenConfiguringTickets.html#adminColorCodingKdsTickets) menu items | Menus > Bulk management > Advanced properties > *`{menu}`* > *`{menu                                                               group}`* > *`{menu item}`* > KDS Color |  | Restaurant Admin > 4.5 Edit Full Menu |
| [Color-code](https://doc.toasttab.com/doc/platformguide/platformKitchenConfiguringTickets.html#adminColorCodingKdsTickets) modifier options | Menus > Bulk management > Advanced properties > *`{menu}`* > *`{menu                                                               group}`* > *`{menu item}`* > *`{modifier group}`* > *`{modifier}`* > KDS Color |  | Restaurant Admin > 4.5 Edit Full Menu |
| Customize names for menu items | Menus > Bulk management > Advanced properties > *`{menu}`* > *`{menu                                                               group}`* > *`{menu item}`* > Kitchen Name |  | Restaurant Admin > 4.5 Edit Full Menu |
| Customize names for modifiers | Menus > Bulk management > Advanced properties > *`{menu}`* > *`{menu                                                               group}`* > *`{menu item}`* > *`{modifier group}`* > *`{modifier}`* > Kitchen Name |  | Restaurant Admin > 4.5 Edit Full Menu |
| Customize other labels | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [Kitchen Names](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#adminKitchenNamesRef) fields |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| Add a the tab name on tickets sent by Quick Order | Front of house > Order screen setup > UI options > [Prompt for tab name? (Quick Order only)](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configPromptTabName): On |  | Web Setup > 6.6 Restaurant Operations Setup |
| Show the dining option on tickets sent by Quick Order when a default dining option is not set | Front of house > Order screen setup > UI options > [Prompt for Dining Option](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configPromptDiningOption): Yes |  | Web Setup > 6.6 Restaurant Operations Setup |
| Always show the dining option | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > Always Print and Show Dining Option: Yes |  | Web Setup > 6.6 Restaurant Operations Setup |

For more information about how to change configuration settings, see [Using Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).

### KDS ticket layout

You can change how order information appears on tickets by setting the options described in the following table.

| If you want to... | Toast Web (All devices) | Toast POS home screen (Each device) | Required Permission |
|---|---|---|---|
| See the check number as the most prominent identifier in ticket headers | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [KDS Ticket Headers](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configKdsTicketHeaders): Check number |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| See the table number (or tab name) as the most prominent identifier in ticket headers | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [KDS Ticket Headers](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configKdsTicketHeaders): Table number |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| See lines with totals for identical items in an order | Front of house > Order screen setup > UI options > [Consolidate menu items](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configCombineItems): On |  | Web Setup > 6.6 Restaurant Operations Setup |
| See every item on its own line | Front of house > Order screen setup > UI options > [Consolidate menu items](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configCombineItems): Off |  | Web Setup > 6.6 Restaurant Operations Setup |
| See identical items consolidated into a single ticket with the quantity number when using separate kitchen tickets for each item | You need to change the following settings:<br>1. Front of house > Order screen setup > UI options > [Consolidate menu items](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configCombineItems): On 2. Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [Individual Item Tickets Order](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configIndividualTickets) > KDS Settings: Display each item on individual tickets... 3. Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [Consolidate Items with Multiple Quantities](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configConsolidateItemsWithMultipleQuantities): Yes |  | Web Setup > Restaurant Operations Setup<br>Web Setup > Kitchen / Dining Room Setup |
| Have a separate ticket for each item (example: tapas-style delivery) | You need to change the following settings:<br>1. Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [Individual Item Tickets](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configIndividualTickets) > KDS Settings: Display each item on individual tickets... 2. Kitchen > Pacing > Meal pacing > Course Pacing: Enable course pacing > Sending Courses: Send all courses individually >[Previous Course Status](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configPreviousCourseStatus): unchecked |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| Have one ticket for all items sent in an order | Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup > [Individual Item Tickets](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configIndividualTickets) > KDS Settings: Display all items... |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| See modifiers on separate lines | Front of house > Order screen setup > UI options > [Modifier display mode](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configModifierDisplayMode): Vertical |  | Web Setup > 6.6 Restaurant Operations Setup |
| See modifiers in a comma separated list | Front of house > Order screen setup > UI options > [Modifier display mode](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configModifierDisplayMode): Horizontal |  | Web Setup > 6.6 Restaurant Operations Setup |
| See modifiers listed by sort order | > 📘 Note > > Using the **Sort Order** setting to sort modifiers on kitchen tickets is in limited release.<br>You need to change the following settings:<br>1. Front of house > Order screen setup > UI options > [Modifier display mode](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configModifierDisplayMode): Vertical or Horizontal 2. On the modifier's details page, a **Sort Order** is assigned. This can also be done on the **Menus > Bulk Management > Advanced properties** page and using the **Show/Hide** dropdown menu to choose **Sort Order**.<br>   > 📘 Note    >    > The assigned **Sort Order** overrides the Modifier group sorting, Modifier display order, and Display Order Priority settings for kitchen tickets. |  | Web Setup > 6.6 Restaurant Operations Setup |
| See modifiers listed by modifier group display ordering priority in a comma-separated list in sequence selected | You need to change the following settings:<br>1. Front of house > Order screen setup > UI options > [Modifier ordering priority](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configModifierOrderingPriority): On<br>   > 📘 Note    >    > For KDS devices using legacy dynamic view and printed kitchen tickets, this setting is always treated as if set to **On**. 2. On the modifier group's details page, the **Display Ordering Priority** setting is assigned. For more information, see [Understanding modifier group display order](https://doc.toasttab.com/doc/platformguide/adminUnderstandingModifierGroupDisplay.html). |  | Web Setup > 6.6 Restaurant Operations Setup |
| See modifiers listed in the same way they were added to the order | Front of house > Order screen setup > UI options > [Modifier group sorting](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configModifierGroupSorting): Display in order modifiers were added |  | Web Setup > 6.6 Restaurant Operations Setup |
| See modifiers listed in the same order as they appear within the modifier group in Toast Web | Front of house > Order screen setup > UI options > [Modifier group sorting](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configModifierGroupSorting): Display in order modifiers are listed in their modifier group |  | Web Setup > 6.6 Restaurant Operations Setup |
| See modifiers on separate lines sequenced first by required modifiers, and then optional modifiers by extra charge amount | Front of house > Order screen setup > UI options > [Modifier display mode](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configModifierDisplayMode): Legacy |  | Web Setup > 6.6 Restaurant Operations Setup |
| See modifiers in a comma-separated list in the order they were added on the orders screen | Front of house > Order screen setup > UI options > [Modifier display mode](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configModifierDisplayMode): Legacy - Flatten |  | Web Setup > 6.6 Restaurant Operations Setup |

For more information about how to change configuration settings, see [Using Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).

### KDS text and ticket size

To assure that every cook can see the tickets on the KDS device clearly, you can change the ticket layout and the text size directly on each device. On the KDS device, select the overflow menu (the ⋮ icon) and choose **KDS appearance**. For more information, see [KDS appearance pane](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKdsAppearancePane).

![A KDS device with the overflow menu and the KDS appearance option selected.](https://doc.toasttab.com/doc/media/KDS_text_ticket_size.png)

To see the rest of the tickets that are waiting to be fulfilled, you swipe the screen from right to left or use the [navigation options](https://doc.toasttab.com/doc/platformguide/platformKDSOverview.html#platformKitchenKdsNavigation) at the bottom of the screen.

> 📘 Note
>
> For legacy KDS view, the **Text Size** option under the overflow menu (the ⋮ icon) is used to change the text size. Changing the text size also changes the size of the tickets and affects how many tickets can appear on the display at one time.

### Printing options for the KDS

Your kitchen can include one or more printers along with your kitchen display system (KDS) devices. (To ensure continuing operation when the Toast devices are in offline mode, at least one kitchen printer is required.) You configure ticket printing by setting the options described in the following table.

> 📘 Note
>
> These options assume that printers are already set up for your restaurant and your KDS devices.
> 
> - In Toast Web, you can choose **Finance > Related > Settings > Printers & cash drawers** and add printers on the **Printers and cash drawers** page. You then choose **Kitchen > Printers, tickets, & KDS devices > Kitchen and ticket setup** and configure printers to the Expediter using the Expediter Printer(s) option. Alternatively, choose **Kitchen > Kitchen stations > Prep stations**, find the row for the prep station you want to change, and choose a printer from the **Ticket Printer** dropdown. These settings determine where orders taken for guests print.
> - On a KDS device, you can choose **Setup > Device Setup > Receipt Printer** and define the primary printer. This setting determines where tickets selected manually on that KDS device print.

| If you want to... | Toast Web (All devices) | Toast POS home screen (Each device) | Required Permission |
|---|---|---|---|
| Print a selected ticket manually | Kitchen > Printers, screens, & KDS devices > Kitchen > [Print On Demand](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configPrintOnDemand): Enable kitchen staff... |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| Print item(s) in a selected ticket manually | Kitchen > Printers, screens, & KDS devices > Kitchen > [Fulfill Items](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configFulfillItems): Enable individual item fulfillment |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| Print tickets automatically on fulfillment |  | Setup > Device Setup > Auto-print Fulfilled Tickets | Device Setup > 7.3 KDS and Order Screen Setup |
| Print expediter tickets automatically when offline | You need to change the following settings:<br>1. Kitchen > Printers, screens, & KDS devices > Kitchen > [Printing Mode](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configPrintingMode): Only print ... when Toast is in offline mode 2. Kitchen > Printers, screens, & KDS devices > Kitchen > [Expediter Printer(s)](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configExpediterPrinters) |  | Web Setup > 6.2 Kitchen / Dining Room Setup |
| Print all expediter tickets automatically | You need to change the following settings:<br>1. Kitchen > Printers, screens, & KDS devices > Kitchen > [Printing Mode](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configPrintingMode): Always print expediter tickets 2. Kitchen > Printers, screens, & KDS devices > Kitchen > [Expediter Printer(s)](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configExpediterPrinters) |  | Web Setup > 6.2 Kitchen / Dining Room Setup |

For more information about how to change configuration settings, see [Accessing the Toast POS Device Setup screen](https://doc.toasttab.com/doc/platformguide/adminConfigureDevice.html) or [Using Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).
