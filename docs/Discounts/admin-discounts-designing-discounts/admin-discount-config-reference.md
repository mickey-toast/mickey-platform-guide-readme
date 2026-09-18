---
title: Discount configuration reference
excerpt: >-
  The following tables describe the fields that are displayed on the discount
  configuration page.
hidden: false
metadata:
  description: >-
    The following tables describe the fields that are displayed on the discount
    configuration page.
---

The following tables describe the fields that are displayed on the discount configuration page.

### Top-level fields

At the top of the discount configuration page are the following fields, which apply to all discounts.

| Basic option | Settings and description |
|---|---|
| **Name of discount** | Sets the name of the discount.<br>The name is used on the discount button on the Toast POS app (unless overridden by the **POS Name** setting) and on sales reports. |
| **Number of discount** | The identifier of the discount. The number is generated when you create the discount. It is not editable.<br>Next to the discount number is the **Copy** option, which allows you to create a copy of the current discount. See [Copying discounts](https://doc.toasttab.com/doc/platformguide/adminCopyingDiscounts.html).<br>For restaurants that use the multi-location module, the discount number is a multi-location ID that the Toast platform uses to determine versions for all of the restaurant locations. You use the **New Version** option to create a new version of the discount. For details about managing versions, see [Creating a version of a configuration entity](https://doc.toasttab.com/doc/platformguide/creatingAVersionOfAConfigurationEntity.html). |
| **Require manager permission for reward redemptions** | This setting displays only if **Permissions Level** in **Advanced Settings** is set to **Manager**.<br>Specifies whether a manager's permission is required to apply third-party (non-Toast) rewards that are linked to this discount.<br>For details, see [Determining who can apply a discount](https://doc.toasttab.com/doc/platformguide/adminDiscountsRequireManager.html). |
| **Target** | Only displays for restaurants that use the multi-location module.<br>Determines the restaurant or group that the discount applies to.<br>For details, see [Discount configurations for multi-location restaurants](https://doc.toasttab.com/doc/platformguide/adminDiscountsTargetsAndOwners.html). |
| **Owner** | Only displays for restaurants that use the multi-location module.<br>Determines the restaurant or group that can configure the discount.<br>For details, see [Discount configurations for multi-location restaurants](https://doc.toasttab.com/doc/platformguide/adminDiscountsTargetsAndOwners.html). |
| **Discount type** | Specifies the discount type:<br>- **Fixed $ Off** - **Fixed % Off** - **Open $ Off** - **Open % Off** - **Buy One Get One** - **Combo** |
| **Limit to Dining Options** | Controls which dining options the discount is available in.<br>The discount will be available in each dining option you specify. In any dining option you do not select, the discount is not available. If you do not specify a dining option, the discount is available in all dining options.<br>For information about dining options, see [Dining options](https://doc.toasttab.com/doc/platformguide/adminDiningOptions.html). |

### Type-specific fields for discounts

When you select the discount type, type-specific fields are displayed below the **Discount type** setting.

#### Fields for fixed and open amount and percent discounts

The following fields display when you set **Discount Type** to one of the fixed or open amount or percent discount types. See [Configuring fixed or open amount or percent discounts](https://doc.toasttab.com/doc/platformguide/adminDiscountsConfigFixedOpenDiscounts.html).

| Fixed discount setting | Options and description |
|---|---|
| **Value** | Displays next to the type field for fixed currency amount and fixed percent discounts.<br>For fixed currency amount discounts, specify the currency amount to discount from the check.<br>For fixed percent amount discounts, specify the percent amount (up to 100%) to discount the check. |
| **Applies to** | How to apply the discount to the check:<br>- **Any item**: The discount applies to any item on the check. No other required item configuration is needed. - **Entire check**: The discount applies to the entire check. Optionally, the discount can be configured so that the check must have one or more required items and/or groups before the discount can apply. - **Specific item/group**: The discount is applied to the specified menu items and/or groups before the discount applies. |
| **Discount will apply to all items except the following items/groups** | For **Applies to=Entire Check** discounts that are not bulk discounts, when you select this check box, you can specify menu items, menu groups, or menus to exclude from the discount.<br>See [Excluding items from a check-level discount](https://doc.toasttab.com/doc/platformguide/adminDiscountsConfigFixedOpenDiscounts.html#adminExclusionDiscounts). |
| **Check must include one of the following items/groups** | For **Applies to=Entire Check** discounts, when you select this check box, you can specify required items for the discount.<br>The required items must be on the check in order for the discount to apply. |
| **Items** | For **Applies to=Specific item/group** discounts, this section allows you to specify the required items for the discount.<br>The required items must be on the check in order for the discount to apply. |

#### BOGO discount fields

The following fields are displayed when you select BOGO as the discount type. See [Configuring a BOGO discount](https://doc.toasttab.com/doc/platformguide/adminDiscountsConfigureBogo.html).

There are also BOGO-specific fields in the [**Advanced Settings** section.](https://doc.toasttab.com/doc/platformguide/adminDiscountConfigReference.html#discountConfigAdvanced)

| BOGO settings | Options and description |
|---|---|
| **Buy Items - Applies to** | The **Applies to** setting determines the buy item type:<br>- **Any item**: The discount applies to any menu item on the check. No other required item configuration is needed. - **Specific item/group**: The check must have one or more required items before the discount applies. |
| **Get Items - Applies to** | The **Applies to** setting determines the get item type:<br>- **Any item**: The get item can be any menu item on the check. No other required item configuration is needed. - **Specific item/group**: The check must have one or more required items before the get item applies. |
| **Get Items - Discount** | Configures the discount for the get item:<br>- The amount to discount. - Whether the discount amount is a **Currency ($)** amount or a **Percentage (%)** amount. - How to select which eligible get item to discount. |

#### Combo discount fields

The following fields display when you set **Discount type** to **Combo**. See [Configuring a combo discount](https://doc.toasttab.com/doc/platformguide/adminDiscountsConfigureCombo.html).

There are also a combo-specific field in the [**Advanced Settings**](https://doc.toasttab.com/doc/platformguide/adminDiscountConfigReference.html#discountConfigAdvanced) section.

| Combo setting | Options and description |
|---|---|
| **Value** | Sets the price of the combo. |
| **Items** | Configures the required items for the discount.<br>The required items must be on the check in order for the discount to apply. |

### Promo codes

The **Promo codes** section contains the list of promo codes for the discount. For details, see [Requiring promo codes for discounts](https://doc.toasttab.com/doc/platformguide/adminDiscountPromoCodes.html).

### Availability

The **Availability** section allows you to configure the dates, days of the week, and times when a discount is available. For details, see [Setting the availability date range for a discount](https://doc.toasttab.com/doc/platformguide/adminDiscountAvailability.html).

| Availability settings | Options and description |
|---|---|
| **Dates Available** | Sets a date range when the discount is available for use.<br>If no date range is configured, the discount is always available, unless there are restrictions based on the days of the week or hours. |
| **Days of the Week Available** | Sets the days of the week when the discount is available for use.<br>You must select at least one day. |
| **Hours Available** | Sets one or more hour ranges when the discount is available.<br>If no hour range is configured, the discount is available at any time of the day, except for restrictions based on the date range or days of the week settings. |

### Advanced settings

| Advanced settings | Options and description |
|---|---|
| **POS Name** | An alternate, shortened name of the discount, used as the text for the discount button on the Toast POS app. |
| **Permissions Level** | Specifies who can apply the discount on the Toast POS app.<br>Either any user can apply the discount, or only a manager can apply the discount.<br>For details, see [Determining who can apply a discount](https://doc.toasttab.com/doc/platformguide/adminDiscountsRequireManager.html). |
| **Allow with other discounts** | Allows a check-level or BOGO discount to apply with other discounts.<br>For details, see [Exclusive and nonexclusive discounts](https://doc.toasttab.com/doc/platformguide/adminDiscountExclusivity.html). |
| **Required Min/Max Check Amount** | Sets minimum and maximum check thresholds. The discount is applied only if the pre-tax total on the check meets the thresholds.<br>For details, see [Configuring required minimum and maximum check totals](https://doc.toasttab.com/doc/platformguide/adminDiscountsMinMax.html). |
| **Auto apply discount** | Only configurable for discounts that are eligible to be auto-applied.<br>Configures the discount to automatically apply to a check.<br>For details, see [Automatically applying discounts](https://doc.toasttab.com/doc/platformguide/adminAutoApplyDiscounts.html). |
| **Discount Reasons** | Used to allow restaurant employees to select a discount reason when they apply a discount.<br>You first select the available discount reasons for the discount.<br>You then choose whether to prompt for a discount reason. If you prompt for a discount reason, you can also require a discount reason and an additional comment.<br>For details, see [Requiring a discount reason for a discount](https://doc.toasttab.com/doc/platformguide/adminDiscountReasons.html). |
| **Total Quantity** | Only displays for combo discounts that are not bulk discounts.<br>The number of times that a combo discount can be applied to an order.<br>For details, see [Configuring a combo discount](https://doc.toasttab.com/doc/platformguide/adminDiscountsConfigureCombo.html). |
| **Required # of Buy Items** | Only displays for BOGO discounts.<br>The minimum number of buy items that the check must have before the bulk discount can apply.<br>For details, see [Configuring a BOGO discount](https://doc.toasttab.com/doc/platformguide/adminDiscountsConfigureBogo.html). |
| **Eligible # of Get Items** | Only displays for BOGO discounts<br>The maximum number of get items that are included in the discount.<br>For details, see [Configuring a BOGO discount](https://doc.toasttab.com/doc/platformguide/adminDiscountsConfigureBogo.html). |
| **Bulk Discount** | Only displays for discounts that are eligible to be bulk discounts.<br>Configures the discount as a bulk discount. For a bulk discount, you also configure the minimum and maximum number of eligible items that the discount is applied to.<br>For details, see [Bulk discounts](https://doc.toasttab.com/doc/platformguide/adminBulkDiscounts.html). |
