---
title: Bulk import tool overview
excerpt: >-
  The bulk import tool allows you to use a comma-separated values (CSV) file to
  import menu changes in bulk to Toast Web. The process for completing a bulk
  menu import is:
hidden: false
metadata:
  description: >-
    The bulk import tool allows you to use a comma-separated values (CSV) file
    to import menu changes in bulk to Toast Web. The process for completing a
    bulk menu import is:
---

> ❗️ Important
>
> Changes made using the bulk import tool are *not reversible*. Also, your restaurant must have the Restaurant Management Essentials, Restaurant Management Pro, or Restaurant Management Enterprise package, or the multi-location module, to access the bulk menu import feature.

The bulk import tool allows you to use a comma-separated values (CSV) file to import menu changes in bulk to Toast Web. The process for completing a bulk menu import is:

1. [Make a copy](https://doc.toasttab.com/doc/platformguide/platformFillingOutTheBulkImportSpreadsheet.html#platformToMakeACopyOfTheBulkImportSpreadsheetTemplate) of a bulk import spreadsheet template.
2. [Fill out a row in the template](https://doc.toasttab.com/doc/platformguide/platformFillingOutTheBulkImportSpreadsheet.html) for each import operation.
3. Download the completed template as a CSV file.
4. [Upload the CSV file](https://doc.toasttab.com/doc/platformguide/platformUploadingTheBulkImportCsvFile.html) into the Toast platform using the **Bulk import tool** in Toast Web.

The tool has three import spreadsheets to choose from:

- [Basic template](https://doc.toasttab.com/doc/platformguide/platformFillingOutTheBulkImportSpreadsheet.html#platformBulkMenuImportBasicTemplate): Use this template to quickly create new menu items, modifier groups, and modifiers with the minimum required information.
- [Item update](https://doc.toasttab.com/doc/platformguide/platformFillingOutTheBulkImportSpreadsheet.html#platformBulkMenuImportItemUpdateTemplate): Use this template to update the name, price, SKU, PLU, description, POS name, kitchen name, and sales category of existing menu items.
- [Advanced template](https://doc.toasttab.com/doc/platformguide/platformFillingOutTheBulkImportSpreadsheet.html#platformBulkMenuImportAdvancedTemplate): Use this template to create and attach menu items, modifier groups, and modifiers, and set advanced settings like button color, SKU, PLU, and others. The import templates use the term *attach* for defining a menu entity's parent in the menu hierarchy. For example, you can attach a menu item to a parent menu group, or a modifier group to a parent menu group or item.

The [Filling out a bulk import spreadsheet](https://doc.toasttab.com/doc/platformguide/platformFillingOutTheBulkImportSpreadsheet.html) section provides detailed information on how to fill out the spreadsheets.

> ❗️ Important
>
> The menu manager tool has a more recent export/import workflow that simplifies the creation of the import CSV file for a limited number of pricing update types. The CSV file created by the menu manager export/import feature functions similarly to the templates described above but it has already been filled out for you, using your existing menus data. For more information, see [Menu manager export](https://doc.toasttab.com/doc/platformguide/platformMenuManagerExport.html).
