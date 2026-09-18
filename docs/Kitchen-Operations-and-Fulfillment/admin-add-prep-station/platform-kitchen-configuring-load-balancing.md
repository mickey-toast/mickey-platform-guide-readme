---
title: Configuring load balancing
excerpt: >-
  You can use load balancing to divide kitchen tickets between prep station KDS
  devices using the same prep station. For information about load balancing, see
  Routing using load…
hidden: false
metadata:
  description: >-
    You can use load balancing to divide kitchen tickets between prep station
    KDS devices using the same prep station. For information about load
    balancing, see Routing using load…
---

> 📘 Note
>
> The load balancing feature is only available for new KDS, previously known as grid view.

You can use load balancing to divide kitchen tickets between prep station KDS devices using the same prep station. For information about load balancing, see [Routing using load balancing](https://doc.toasttab.com/doc/platformguide/platformKitchenRoutingUsingLoadBalancing.html).

To start using load balancing, you need to:

1. [Create at least two load-balancing groups in Toast Web](https://doc.toasttab.com/doc/platformguide/platformKitchenConfiguringLoadBalancing.html#platformKitchenCreatingLoadBalancingGroups).
2. [Turn on start queue in Toast Web](https://doc.toasttab.com/doc/platformguide/platformKitchenConfiguringLoadBalancing.html#platformKitchenUsingStartQueueWithLoadBalancing).
3. [Choose a load-balancing group on the KDS device.](https://doc.toasttab.com/doc/platformguide/platformKitchenConfiguringLoadBalancing.html#platformKitchenAssigningLoadBalancingGroupToKds)

You can modify or archive load-balancing groups after they are created. For more information, see [Editing or archiving load-balancing groups](https://doc.toasttab.com/doc/platformguide/platformKitchenConfiguringLoadBalancing.html#platformKitchenEditingArchivingLoadBalancingGroups). For an example workflow of a kitchen using load balancing, see [KDS workflow using load balancing](https://doc.toasttab.com/doc/platformguide/platformKdsWorkflowLoadBalancing.html).

### Creating load-balancing groups

First, create at least two load-balancing groups. Tickets can then be split between the two groups.

**To set up load-balancing groups**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).
2. Go to **Kitchen** > **Kitchen stations** > **Load balancing**. The **Load balancing** page opens.

   > 📘 Note
   >
   > When initially opening this page, you are prompted to create two load-balancing groups.
3. Select **+ Create New Group**. The **Create group** pane opens.
4. Add a **Group name**.

   > 📘 Note
   >
   > The load-balancing group name appears in two places on the KDS device:
   > 
   > - On prep station KDS devices, it is part of the prep station name, which includes the prep stations that are assigned to that device.
   > - On expediter KDS devices, it is next to the item name after it is claimed by the load-balancing group.
   > 
   > Toast Support recommends keeping the name short.
5. If needed, use the **Available at (Target)** setting to select a target location. For more information about targets, see [Targets](https://doc.toasttab.com/doc/platformguide/targets.html).
6. Select **Create group**. The pane closes and the group is added to the list of load-balancing groups.
7. Save and publish your changes.

### Using start queue with load balancing

If needed, turn on start queue. For information about start queue, see [Using start queue](https://doc.toasttab.com/doc/platformguide/platformKdsStartQueue.html).

> 📘 Note
>
> Depending on your kitchen setup, you will need the **Start queue** setting to be either **On - Manually turn on for each device** or **On - All devices at this restaurant**. For examples about how you can use start queue with load balancing, see [Example load balancing scenarios](https://doc.toasttab.com/doc/platformguide/platformKitchenRoutingUsingLoadBalancing.html#platformKitchenExampleLoadBalancingScenarios).

### Assigning a load-balancing group to a KDS device

Next, assign a load-balancing group to a prep station KDS device. Depending on your kitchen setup, you can also choose to configure the KDS device to claim tickets for the load-balancing group. That prep station KDS device is now the lead claiming device. Lead claiming devices can claim tickets and are marked with **Claim** next to the prep station KDS device name.

![A prep station KDS showing the Claim label indicating it is a lead claiming device, and the load-balancing group name added to the prep station name.](https://doc.toasttab.com/doc/media/kitchen-kds-load-balancing-lead-claiming-device.png)

> 📘 Note
>
> A prep station KDS device that is configured to be a lead claiming device must also use start queue.

**To assign a load-balancing group to a KDS device**

> 📘 Note
>
> You can only configure load balancing for prep station KDS devices.

1. On your KDS device, access the [**Device Setup** screen](https://doc.toasttab.com/doc/platformguide/adminConfigureDevice.html).
2. Go to the **Kitchen Setup** section.
3. Select **Load Balancing**. The load balancing screen opens.
4. Select **Load-balancing group**. The selection screen opens.
5. Choose the load-balancing group that best fits the KDS device.
6. Select **Save**. You are returned to the load balancing screen.
7. If you want to make the current KDS a lead claiming device, turn on the **Lead claiming device** setting.

   > 📘 Note
   >
   > Toast Support recommends using one lead claiming device for each load-balancing group.
8. Return to the KDS screen.

### Editing or archiving load-balancing groups

After you create a load-balancing group, you can choose to edit or to archive it using the overflow menu (the ⋮ icon).

**To edit the load-balancing group**

1. To open the **Edit group** pane, choose to:

   - Select the name of the load-balancing group from under the **Group Name** column, or
   - Select the overflow menu (the ⋮ icon) and select **Edit**.

   The **Edit group** pane opens.
2. Update either the **Group name** or the **Available at (Target)** values.
3. Select **Save**. The **Edit group** pane closes and the changes are reflected in the load-balancing group table.

   ![The Load balancing page in Toast Web, with the load-balancing group table.](https://doc.toasttab.com/doc/media/kitchen-kds-load-balancing-tw-page-table.png)
4. Save and publish your changes.

To archive a load-balancing group, select the overflow menu (the ⋮ icon) and select **Archive**. If you are showing archived groups, the **Status** column shows **ARCHIVED**.

Archived load-balancing groups are initially hidden, but are shown by selecting the **Show Archived** toggle. Archiving a group prevents you from choosing it on a KDS device. If you archive a group and publish your changes when a KDS device currently uses that group, load balancing is disabled on that device until you select a new load-balancing group.

> 📘 Note
>
> The **Status** column shows whether a group is **ACTIVE**, which means it can be used by KDS devices, or **ARCHIVED**, which means it cannot be used by KDS devices.

An archived load-balancing group can be unarchived. To unarchive a load-balancing group, select the overflow menu (the ⋮ icon) and select **Unarchive**.
