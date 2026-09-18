---
title: Manually purging closed orders
excerpt: >-
  If you choose to manually initiate a closed order purge, the process is
  effectively the same as when the order purger service runs with the exception
  of the threshold setting,…
hidden: false
metadata:
  description: >-
    If you choose to manually initiate a closed order purge, the process is
    effectively the same as when the order purger service runs with the
    exception of the threshold setting,…
---

If you choose to manually initiate a closed order purge, the process is effectively the same as when the [order purger service](https://doc.toasttab.com/doc/platformguide/adminConfiguringTheOrderPurgerService.html) runs with the exception of the threshold setting, which is ignored. A manual purge will run even if the total number of orders in any state is less than the configured threshold.

**To manually purge closed orders**

1. At the top of the screen, tap **Switch User**.
2. Tap the overflow menu (⋮) in the upper-right of the screen.
3. Tap **Clear Closed Orders** in the menu.
4. Repeat this process on all devices that require it.
