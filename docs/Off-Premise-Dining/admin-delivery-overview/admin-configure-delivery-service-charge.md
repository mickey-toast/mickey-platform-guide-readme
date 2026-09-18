---
title: Configuring a delivery service charge
excerpt: >-
  You can create and apply a service charge to delivery orders. The service
  charge is automatically applied to all delivery orders.
hidden: false
metadata:
  description: >-
    You can create and apply a service charge to delivery orders. The service
    charge is automatically applied to all delivery orders.
---

You can create and apply a service charge to delivery orders. The service charge is automatically applied to all delivery orders.

**To configure a service charge for delivery orders**

1. [Access Toast Web](https://doc.toasttab.com/doc/platformguide/adminAccessToastAdminBackend.html).
2. Choose **Takeout & delivery > Availability > Takeout/delivery** to open the **Takeout/delivery** page.
3. In the **Delivery fee** section, select the **Configure delivery service fees** link to open the **Service charges** page. You can also navigate to this page by choosing **Finance > Related > Settings > Service charges & fees**.
4. Select the **+ Add** button.
5. Enter your service charge information. For more information about service charges, see [Configuring service charges](https://doc.toasttab.com/doc/platformguide/adminServiceChargeCreate.html).
6. Go to the **Delivery** option. Select **Yes** to open the advanced **Delivery configuration** section.

   > 📘 Note
   >
   > A delivery service charge is applied to checks that have their dining behavior set to **Delivery**.

   - **Waive fee threshold**: Enter a threshold (as a dollar amount) that determines whether to waive the delivery service charge. The service charge is waived if the pre-discount amount of the check is greater than or equal to this amount. If you do not enter a waive fee threshold or the threshold is $0.00, the fee is not waived.

      Do not set a **Waive fee threshold** if you have set an **Apply after amount threshold** amount.

   - **Delivery distance threshold**: Enter the distance value that determines whether to apply the delivery service charge. This fee is only applied if the distance from the restaurant to the delivery address is greater than or equal to this value and the dining behavior is set to **Delivery**. The **Delivery distance threshold** does not apply to TDS orders.
7. Select the **Save** button to save your changes and then the **Publish Now** button to publish your changes.

   The new service charge appears on the **Service charges** page. On the **Service charges** page, you can edit charges, apply charges to other dining options, reorder charges, or archive charges.
