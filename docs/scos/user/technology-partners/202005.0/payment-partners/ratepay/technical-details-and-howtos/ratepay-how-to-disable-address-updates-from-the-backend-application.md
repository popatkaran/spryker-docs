---
title: RatePay - How to Disable Address Updates from the Backend Application
description: Disable address updates from the backend application for Ratepay.
originalLink: https://documentation.spryker.com/v5/docs/ratepay-disable-address-updates
originalArticleId: c76fe229-57f4-421b-8f40-b0bd3c357907
redirect_from:
  - /v5/docs/ratepay-disable-address-updates
  - /v5/docs/en/ratepay-disable-address-updates
---

To disable updates on addresses from the backend application, follow the steps described below:

**Step 1**:

* Overwrite on project side
`/vendor/spryker/spryker/Bundles/Sales/src/Spryker/<br>Zed/Sales/Presentation/Detail/boxes/addresses.twig`
* Remove ' `Edit`' button

**Step 2**:

* Overwrite on project side
`/vendor/spryker/spryker/Bundles/Sales/src/Spryker/<br>Zed/Sales/Communication/Controller/EditController.php`
* Disable ' `addressAction`'