---
title: Manually assigning applicable taxes
excerpt: >-
  The preferred technique for managing taxes is to manually assign the master
  versions of your tax rates to your menus. With this configuration, the correct
  version of the tax…
hidden: false
metadata:
  description: >-
    The preferred technique for managing taxes is to manually assign the master
    versions of your tax rates to your menus. With this configuration, the
    correct version of the tax…
---

The preferred technique for managing taxes is to manually assign the master versions of your tax rates to your menus. With this configuration, the correct version of the tax will be applied to a menu, depending on location. For example, assuming the following tax rates, if the current location is Boston, the state tax would be 6.25% while when the current location is Atlanta, the state tax is 4%.

![](https://doc.toasttab.com/doc/media/tax_rates_no_defaults.PNG)

**To assign tax rates manually**

1. Choose **Menus > Menu management > Tax rates** setup to open the **Tax rates** page.
2. Use the **You are viewing** menu to show the tax rates for the corporate restaurant group (this group should show all locations). See [Filtering pages](https://doc.toasttab.com/doc/platformguide/filteringPagesForSpecificRestaurantGroupsAndLocations.html) for information on the **You are viewing** menu.
3. Make sure your tax rates are not marked as default.
4. Choose **Menus > Bulk management > Advanced properties** to open the **Advanced properties** page.
5. Use the **You are viewing** menu to view the menus you want to assign taxes to.
6. Select the **Show/Hide** menu, scroll down to the **Taxes** section and check the **Applicable Taxes** option to display that column on the **Advanced properties** page.
7. In the row for the menu you want to apply taxes to, select the **Applicable Taxes** field.
8. All of the master tax rates you have created are listed below the line in the **Applicable Taxes** field. Select a master tax rate to select it and apply its taxes to this menu. To deselect a master tax rate, select it again to remove the checkmark. Check all of the master tax rates that should apply to this menu, for example:

   ![](https://doc.toasttab.com/doc/media/tax_rates_manually_assigned_adv_props_page.PNG)
9. Select **Save**.
10. Repeat these steps for each menu.
11. Publish your changes using the **Publish config** page. See [Publishing changes for multiple locations](https://doc.toasttab.com/doc/platformguide/publishingChangesForMultipleLocations.html) for information on accessing and using that page.
