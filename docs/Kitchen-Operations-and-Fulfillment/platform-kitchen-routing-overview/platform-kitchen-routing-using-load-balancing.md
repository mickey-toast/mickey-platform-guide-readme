---
title: Routing using load balancing
excerpt: >-
  In kitchen setups where you assign the same prep station to multiple KDS
  devices, items assigned to those prep stations are shown on multiple devices.
  To avoid duplicated work…
hidden: false
metadata:
  description: >-
    In kitchen setups where you assign the same prep station to multiple KDS
    devices, items assigned to those prep stations are shown on multiple
    devices. To avoid duplicated work…
---

> 📘 Note
>
> The load balancing feature is only available for new KDS, previously known as grid view.

In kitchen setups where you assign the same prep station to multiple KDS devices, items assigned to those prep stations are shown on multiple devices. To avoid duplicated work and keep tickets shown on prep station KDS devices to a minimum, you can use load balancing. Load balancing is a way to divide tickets between prep stations and show specific tickets at specific prep station KDS devices. This allows KDS devices with the same prep station to divide the work. Load balancing uses load-balancing groups and assigns each prep station KDS device to one of these groups to divide tickets.

Load balancing uses start queue to claim a ticket for the load-balancing group. Unclaimed tickets, or unstarted tickets, appear on all prep station KDS devices configured to claim tickets. Once a ticket is claimed for the load-balancing group by starting it, the ticket disappears from all prep station KDS devices not in that load-balancing group. You can choose a prep station KDS device as a lead claiming device, which limits claiming tickets for a load-balancing group to that specific prep station KDS device.

Expediter KDS devices automatically see all items. They cannot choose a load-balancing group or be chosen as a lead claiming device.

You do not need to use [start queue](https://doc.toasttab.com/doc/platformguide/platformKdsStartQueue.html#platformKdsStartQueueOverview) on all prep station KDS devices in the load-balancing group. If there is a prep station KDS device in the load-balancing group that does not use start queue, the ticket only appears after it is claimed or, if using assembly lines, when it is fulfilled by the previous prep station KDS device in the assembly line.

> 📘 Note
>
> If using [assembly lines](https://doc.toasttab.com/doc/platformguide/platformKDSRoutingUsingAssemblyLines.html), Toast Support recommends choosing the first prep station KDS device in the line as the lead claiming device. Toast Support recommends not choosing more than one claiming device for a load-balancing group.

For information about how to set up load balancing, see [Configuring load balancing](https://doc.toasttab.com/doc/platformguide/platformKitchenConfiguringLoadBalancing.html). For an example workflow of a kitchen using load balancing, see [KDS workflow using load balancing](https://doc.toasttab.com/doc/platformguide/platformKdsWorkflowLoadBalancing.html).

### Example load balancing scenarios

It is important to understand how you want to use load balancing in the kitchen. The existing settings and setup can influence which prep station KDS devices are included in load-balancing groups and use start queue. Here are a few example kitchen setups and load-balancing configurations.

#### Items are assigned to a single prep station

A kitchen prepares items at either the Drinks or Food prep station. When the kitchen gets busy, it opens second Drinks and Food prep stations. All four prep stations have KDS devices.

To split the work between the two stations, the location uses two load-balancing groups. *Group A* is used by prep station KDS devices that are always in use. *Group B* is used by prep station KDS devices opened when the kitchen gets busy. Each load-balancing group includes a Drinks and a Food prep station KDS device.

*Group A* includes:

- A Drinks prep station KDS device, which claims Drinks prep station tickets for *Group A*.
- A Food prep station KDS device, which claims Food prep station tickets for *Group A*.

Both KDS devices use start queue and are lead claiming devices.

*Group B* includes:

- A Drinks prep station KDS device, which claims Drinks prep station tickets for *Group B*.
- A Food prep station KDS device, which claims Food prep station tickets for *Group B*.

Both devices use start queue and are lead claiming devices.

If a prep station KDS device in *Group A* is too busy to claim a ticket, it can be claimed by the prep station KDS device in *Group B*. The ticket is removed from the prep station KDS device in *Group A*.

Though Toast Support generally recommends using one lead claiming device for each load-balancing group, in this example, one prep station KDS device in a load-balancing group cannot see the tickets for the other prep station KDS device.

For example, the Drinks prep station KDS device cannot see and claim Food prep station tickets. If the Food KDS prep station was not a lead claiming device, no tickets would appear because the lead claiming device (the Drinks prep station KDS device) cannot claim Food prep station tickets.

#### Items are prepared at multiple prep stations simultaneously

A location has five prep stations: Bakery, Cold, Drinks, Grill/Fry, and Hot. All items that use the Grill/Fry prep station also use the Hot prep station. The Grill/Fry and Hot prep stations are the busiest in the kitchen, so there are two prep station KDS devices used for each of these prep stations. To avoid duplicating work by showing the same prep station tickets on two KDS devices, the location uses load balancing.

The location uses two load-balancing groups, *East* and *West*. Each load-balancing group includes a Grill/Fry and a Hot prep station KDS device. The Hot prep station KDS devices use start queue and are the lead claiming devices. The Grill/Fry prep station KDS devices do not use start queue.

*East* includes:

- A Hot prep station KDS device, which claims Hot prep station tickets for *East*.

   > 📘 Note
   >
   > All Grill/Fry prep station items are also assigned to the Hot prep station. When a ticket is claimed at the Hot prep station KDS device, the Grill/Fry items in that ticket appear on the Grill/Fry prep station KDS device.
- A Grill/Fry prep station KDS device, which sees and works on Grill/Fry prep station tickets claimed for *East*.

*West* includes:

- A Hot prep station KDS device, which claims Hot prep station tickets for *West*.

   > 📘 Note
   >
   > All Grill/Fry prep station items are also assigned to the Hot prep station. When a ticket is claimed at the Hot prep station KDS device, the Grill/Fry items in that ticket appear on the Grill/Fry prep station KDS device.
- A Grill/Fry prep station KDS device, which sees and works on Grill/Fry prep station tickets claimed for *West*.

The Bakery, Cold, and Drinks prep stations each have a single prep station KDS device and are not part of a load-balancing group. Items assigned to these prep stations appear on their corresponding prep station KDS devices when they are sent to the kitchen.

If the Hot prep station KDS device in *East* is too busy to claim a ticket, it can be claimed by the Hot prep station KDS device in *West*. The ticket is removed from the Hot prep station KDS device in *East* and, if the item claimed is also assigned the Grill/Fry prep station, appears on the Grill/Fry prep station KDS device in *West*.

#### Items are prepared at multiple prep stations in an assembly line

A pizza restaurant uses an assembly line with prep stations Dough, Sauce, Toppings, and Bake, in that order. There are four prep station KDS devices, one for each of these prep stations. On Friday nights it gets busier than usual, so the location opens a second assembly line with the same prep station KDS device setup.

The location uses a load-balancing group for each of these assembly lines, called *Line A* and *Line B*. Each group has four prep station KDS devices, one each for the Dough, Sauce, Toppings, and Bake prep stations. The Dough prep station KDS devices in both load-balancing groups are the lead claiming device and use start queue because all pizza items use the Dough prep station.

*Line A* includes:

- A Dough prep station KDS device, which claims Dough prep station tickets for *Line A*.

   > 📘 Note
   >
   > All items for the rest of the prep stations in the assembly line also use at least the Dough prep station, so all prep station items in this assembly line appear at the Dough prep station.
- Once the item is fulfilled at the Dough prep station KDS device, it appears at the next *Line A* prep station in the assembly line. For example, if an item is assigned the Sauce prep station, it appears at the Sauce prep station KDS device for *Line A*. The item continues through the assembly line using the prep station KDS devices in *Line A*.

*Line B* includes:

- A Dough prep station KDS device, which claims Dough prep station tickets for *Line B*.

   > 📘 Note
   >
   > All items for the rest of the prep stations in the assembly line also use at least the Dough prep station, so all prep station items in this assembly line appear at the Dough prep station.
- Once the item is fulfilled at the Dough prep station KDS device, it appears at the next *Line B* prep station in the assembly line. For example, if an item is assigned the Sauce prep station, it appears at the Sauce prep station KDS device for *Line B*. The item continues through the assembly line using the prep station KDS devices in *Line B*.

If the Dough prep station KDS device in *Line A* is too busy to claim a ticket, it can be claimed by the Dough prep station KDS device in *Line B*. The ticket is removed from the Dough prep station KDS device in *Line A*. When the ticket is fulfilled at *Line B*, it appears at the next prep station KDS device in the assembly line for *Line B*.

For more information on how assembly lines work, see [Routing using assembly lines](https://doc.toasttab.com/doc/platformguide/platformKDSRoutingUsingAssemblyLines.html).
