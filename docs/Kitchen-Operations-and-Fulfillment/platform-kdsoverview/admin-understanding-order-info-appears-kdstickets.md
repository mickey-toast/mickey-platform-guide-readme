---
title: Understanding how order information appears on KDS tickets
excerpt: >-
  The order information that specifies the table or guest name for an order
  displays according to what was provided.
hidden: false
metadata:
  description: >-
    The order information that specifies the table or guest name for an order
    displays according to what was provided.
---

The order information that specifies the table or guest name for an order displays according to what was provided.

1. If only the tab name is available, **Tab: <tab name>** is shown.
2. If only the table number is available, **Table <table number>** is shown.
3. If both tab name and table numbers are available, **Table <table number>, Tab: <tab name>** is shown.
4. If neither the tab name nor table numbers are available, then the guest's first name and last name are shown. These are taken from the `Customers` object.
5. If the table number, tab name, and guest name are unavailable, only the check number displays.

> 📘 Note
>
> Whether the table or guest information appears before or after the check number depends on the [KDS Ticket Headers](https://doc.toasttab.com/doc/platformguide/adminKitchenDiningRoomReference.html#configKdsTicketHeaders).

The following example shows an order ticket on the KDS device with both a tab name and a table number.

![An example of a KDS ticket that has both a table number and a tab name.](https://doc.toasttab.com/doc/media/KDS_table_tab_name.png)

The following example shows an order ticket on the KDS device with the guest's first name and last name, submitted using online ordering.

![An example of a KDS ticket that has only the guest name.](https://doc.toasttab.com/doc/media/KDS_guest_name.png)

To prompt for a tab name on the Toast POS app, see [**Prompt for tab name? (Quick Order only)**](https://doc.toasttab.com/doc/platformguide/adminUiOptionsReference.html#configPromptTabName).
