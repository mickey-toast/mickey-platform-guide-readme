---
title: Assigning restaurant access
excerpt: >-
  The Restaurant Access tab on an employee's details page allows you to quickly
  give an employee access to multiple locations in your enterprise. An employee
  must have restaurant…
hidden: false
metadata:
  description: >-
    The Restaurant Access tab on an employee's details page allows you to
    quickly give an employee access to multiple locations in your enterprise. An
    employee must have restaurant…
---

The **Restaurant Access** tab on an employee's details page allows you to quickly give an employee access to multiple locations in your enterprise. *An employee must have restaurant access to a location in order to use that restaurant's Toast POS devices.*

![](https://doc.toasttab.com/doc/media/mjm-restaurant-access-tab.PNG)

On the **Restaurant Access** tab, you select the portion of your restaurant group hierarchy that the employee should have access to and then select **Save**. After saving, you return to the **Jobs and Permissions** tab, where you see entries in the **Access Permissions** area that correspond to the locations you chose on the **Restaurant Access** tab. For example, choosing Northeast in the **Restaurant Access** tab shown above results in access permission entries for the Boston, Burlington, and NYC locations on the **Jobs and Permissions** tab.

![](https://doc.toasttab.com/doc/media/mjm-jobs-and-permissions-tab.PNG)

Note that the access permission entries are for *locations only* (Boston, Burlington, and NYC in our example). Restaurant group-level permissions (that is, permissions to the Northeast restaurant group itself) are given using another workflow introduced below.

You can select a location's entry in the **Access Permissions** area to see which permissions the employee has at that location. These permissions reflect the jobs the employee has been assigned and any explicit permission overrides you have specified. For a complete discussion of the **Access Permissions** area, see [Understanding the Jobs and Permissions tab in enterprise environments](https://doc.toasttab.com/doc/platformguide/adminUnderstandingTheJobsAndPermissionsTabInEnterpriseEnvironments.html).

To modify the jobs or permissions an employee has at a given location, you must have the proper permissions yourself, as described in [Editing an employee's permissions](https://doc.toasttab.com/doc/platformguide/adminEditingEmployeeInformationJobsAndPermissionsInEnterprises.html#adminEditingAnEmployeesPermissions). For employees, such as managers, that require access to multiple locations, you may also need to give them restaurant-group level permissions. Restaurant-group level permissions allow the employee to edit configuration entities (menus, menu items, prep stations, void reasons, and so on) in Toast Web that are [owned](https://doc.toasttab.com/doc/platformguide/ownersAndPermissions.html) by restaurant groups. They also allow the employee to view reports for groups of restaurants. For more information, see [Assigning restaurant group-level permissions](https://doc.toasttab.com/doc/platformguide/adminAssigningRestaurantGroupLevelPermissions.html).

If you remove an employee's restaurant access to the session restaurant (that is, the restaurant you are currently logged into), you are notified that the employee has been removed and the employee is no longer accessible in the session restaurant. If the employee has access to other restaurants, you can log into one of those to see and manage the employee's details.
