---
title: Viewing the 86 report
excerpt: >-
  The Reports > Menus > 86 Report is a useful tool you can use to decide which
  menu items to reorder. The 86 Report provides the following information:
hidden: false
metadata:
  description: >-
    The Reports > Menus > 86 Report is a useful tool you can use to decide which
    menu items to reorder. The 86 Report provides the following information:
---

The **Reports > Menus > 86 Report** is a useful tool you can use to decide which menu items to reorder. The **86 Report** provides the following information:

- Menu items that have an inventory status of **Out of Stock** (that is, menu items that have been 86ed). **Out of Stock** menu items are always reported.
- Menu items that have an inventory status of **Quantity** and have a remaining quantity less than or equal to a threshold. You set the threshold by specifying a number in the **Threshold Value** field and selecting **Submit**.

In the report, the **Quantity Remaining** column indicates the number of items left in stock.

In this example which has a **Threshold Value** of 10, the `Wings` and `Grilled Salmon` menu items are out of stock (**Quantity Remaining** is 0 for both) and the `Pie` menu item is running low (**Quantity Remaining** is 4).

![The Inventory property of a menu item.](https://doc.toasttab.com/doc/media/item-inventory-86-report.png)

Note that if you had set the **Threshold Value** to 3, the `Pie` menu item would not be listed because its remaining quantity of 4 is greater than the threshold.
