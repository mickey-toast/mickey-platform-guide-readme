---
title: Configuring the order purger service
excerpt: >-
  The order purger service runs every five minutes and counts the total number
  of orders in any state (open, paid, or closed). If that total number exceeds
  the defined Order…
hidden: false
metadata:
  description: >-
    The order purger service runs every five minutes and counts the total number
    of orders in any state (open, paid, or closed). If that total number exceeds
    the defined Order…
---

The order purger service runs every five minutes and counts the total number of orders in any state (open, paid, or closed). If that total number exceeds the defined **Order Purge Threshold**, the order purger iterates over the orders, marks those that are closed and can be purged from the device, and then removes the marked orders from the device. By default, the **Order Purge Threshold** is 800 total orders. Reducing this threshold causes the order purger to purge orders more frequently because the threshold gets met more frequently.

> ❗️ Important
>
> You should work with Toast support to determine an appropriate **Order Purge Threshold** for your restaurant. Once you have a threshold value, use the instructions below to set the threshold for each of your Toast POS devices.

**To set the order purger threshold**

1. Access [Device Setup](https://doc.toasttab.com/doc/platformguide/adminConfigureDevice.html).
2. Tap **Order Purge Threshold**.
3. Enter the threshold value and tap **Continue**.
4. Repeat these steps on all Toast POS devices, using the same order purge threshold value.
