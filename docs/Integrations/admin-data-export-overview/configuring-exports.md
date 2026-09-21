---
title: Configuring exports
excerpt: >-
  You can use the Data Exports page in Toast Web to configure the Toast platform
  to write data export files containing information about your restaurant
  operations. To open the…
hidden: false
metadata:
  description: >-
    You can use the Data Exports page in Toast Web to configure the Toast
    platform to write data export files containing information about your
    restaurant operations. To open the…
---

You can use the **Data Exports** page in Toast Web to configure the Toast platform to write data export files containing information about your restaurant operations. To open the **Data Exports** page, choose **Reports > Settings > Data Exports** from [Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).

To use the **Data Exports** page to [modify the data export](https://support.toasttab.com/article/Automated-Nightly-Data-Export-1492723819691) setup for your restaurant or restaurant group, you must have the **8.3 Data Export Config** permission. This permission gives you access to the **Data Exports** page in Toast Web. If the restaurant you are currently viewing is part of a restaurant group, the export configurations you define on this page apply to all restaurants in that group.

> 📘 Note
>
> If your restaurant or restaurant group is not configured to generate data export files, you must contact Toast support to set up your data export access before you can configure your exports.

On the **Data Exports** page, you see a list of exportable data types, for example, Orders, Checks, Payments, and so on. To include a data type in your export, select the **Enabled** option for the data type. When you select **Enabled**, a list of columns associated with that data type is shown, allowing you to include or exclude the specific data you need for the data type. Toggle the inclusion of a column by selecting the check mark next to it. Note that a data type's columns are not displayed unless the data type itself is enabled.

![The Data Exports page displaying data options.](https://doc.toasttab.com/doc/media/data-export-configuration-screen.png)

### Configuring the order of data export columns

You can reorder the columns in each data type by selecting the grid box in the far left column and moving it up or down into place. The order of the columns in the data export file reflects the order you arrange in Toast Web.

![The Data Exports page emphasizing the grid boxes on the left column.](https://doc.toasttab.com/doc/media/data-export-grid-box.png)

The following reports contain formatting that do not allow for columns to be reordered:

- Accounting Data Export
- Menu Data Export
