---
title: Kitchen printers
excerpt: >-
  For restaurants using kitchen printers and not KDS devices, when an outage is
  triggered by an internet service provider or Toast platform cloud-based
  service outage, Toast POS…
hidden: false
metadata:
  description: >-
    For restaurants using kitchen printers and not KDS devices, when an outage
    is triggered by an internet service provider or Toast platform cloud-based
    service outage, Toast POS…
---

For restaurants using kitchen printers and not KDS devices, when an outage is triggered by an internet service provider or Toast platform cloud-based service outage, Toast POS devices continue to send orders to the kitchen printers. Online orders are not received by the restaurant when offline. To add kitchen printers, see [Adding a kitchen printer](https://doc.toasttab.com/doc/platformguide/adminAddKitchenPrinter.html).

If an outage is caused by a local network issue, the Toast POS device cannot send tickets to the kitchen printers.

If autofiring is configured, when the connection is restored for all outage types, the Toast platform prints all online orders. This includes all online orders sent during the outage that were not received by the restaurant.
