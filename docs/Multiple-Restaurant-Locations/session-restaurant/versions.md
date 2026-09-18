---
title: Versions
excerpt: >-
  To allow your locations to share some aspects of a configuration entity while
  maintaining the ability to override other aspects, you can use versions. For
  example, consider the…
hidden: false
metadata:
  description: >-
    To allow your locations to share some aspects of a configuration entity
    while maintaining the ability to override other aspects, you can use
    versions. For example, consider the…
---

To allow your locations to share some aspects of a configuration entity while maintaining the ability to override other aspects, you can use versions. For example, consider the following Seafood menu group made up of four menu items, Lobster, Trout, Salmon, and Shrimp:

![](https://doc.toasttab.com/doc/media/original_version.png)

Now imagine that your Northeast locations do not sell shrimp and your Southeast locations do not sell lobster. To create a scenario where your locations share as much configuration as possible, you create an initial version of the Seafood menu group that contains all of your seafood items and then you create two additional versions of that menu group, one that omits shrimp and is used by the Northeast locations and another that omits lobster and is used by the Southeast locations. The same menu items are used by all three versions and the menu item details (for example, sizes, prices, and so on) are controlled at the corporate level. Each version of the Seafood menu group includes or excludes menu items as appropriate for different locations.

![](https://doc.toasttab.com/doc/media/multiple_versions.png)

Using this technique of defining an original version of a configuration entity and then creating additional versions that override or modify some aspect of the original version allows you to share the bulk of your configuration across locations while maintaining the flexibility to define location-specific versions as needed. In cases where all of your locations can share the same configuration entity, you only need to create an initial version of the entity and configure it to be used by all locations.
