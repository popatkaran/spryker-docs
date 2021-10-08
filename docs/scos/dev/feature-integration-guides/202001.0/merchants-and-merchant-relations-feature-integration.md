---
title: Merchants and Merchant Relations feature integration
originalLink: https://documentation.spryker.com/v4/docs/merchant-merchant-relations-feature-integration
originalArticleId: 9a8a2344-0a34-4bb4-9b71-507becca0a9c
redirect_from:
  - /v4/docs/merchant-merchant-relations-feature-integration
  - /v4/docs/en/merchant-merchant-relations-feature-integration
---

The Merchants and Merchant Relations feature is shipped with following modules:

| Module | Description |
| --- | --- |
| [Merchant](https://github.com/spryker/spryker/tree/master/Bundles/Merchant) | Implements logic of Merchants (adding, editing, removal). |
| [MerchantGui](https://github.com/spryker/spryker/tree/master/Bundles/MerchantGui) | Provides table with merchants along with the Create and Edit merchants pages in the Administration Interface. |
| [MerchantRelationship](https://github.com/spryker/spryker/tree/master/Bundles/MerchantRelationship) | Implements logic of merchant relations. |
| [MerchantRelationshipGui](https://github.com/spryker/spryker/tree/master/Bundles/MerchantRelationshipGui) | Provides a table with merchant relations along with the Create and Edit merchant relations pages in the Administration Interface. |
| [MerchantDataImport](https://github.com/spryker/spryker/tree/master/Bundles/MerchantDataImport) | Implements an importer for merchants. |
| [MerchantRelationshipDataImport](https://github.com/spryker/spryker/tree/master/Bundles/MerchantRelationshipDataImport) | Implements an importer for merchant relations. |

To install the Merchants and Merchant relations feature, follow the steps below:

1. Install necessary modules using composer:
Update existing and install the required modules:

```bash
composer update "spryker/*" "spryker-shop/*"
```

```bash
composer require spryker/company-business-unit-data-import:"^0.2.0" spryker/merchant:"^1.0.0" spryker/merchant-data-import:"^0.1.0" spryker/merchant-gui:"^1.0.0" spryker/merchant-relationship:"^1.0.0" spryker/merchant-relationship-data-import:"^0.1.0" spryker/merchant-relationship-gui:"^1.0.0" --update-with-dependencies
```

2. Run the commands:

```bash
console transfer:generate
console propel:install
navigation:build-cache
```

3. Add plugins to Zed `DataImportDependencyProvider`:

| Module | Plugin | Description | Method in Dependency Provider |
| --- | --- | --- | --- |
| `DataImport` | `MerchantDataImportPlugin` | Imports merchants. | `getDataImporterPlugins` |
| `DataImport` | `MerchantRelationshipDataImportPlugin` | Imports merchant relations. | `getDataImporterPlugins` |

**src\Pyz\Zed\DataImport\DataImportDependencyProvider.php**

```php
...
use Spryker\Zed\MerchantDataImport\Communication\Plugin\MerchantDataImportPlugin;
use Spryker\Zed\MerchantRelationshipDataImport\Communication\Plugin\MerchantRelationshipDataImportPlugin;
...									
protected function getDataImporterPlugins(): array
{
    return [
        ...
        new MerchantDataImportPlugin(),
        new MerchantRelationshipDataImportPlugin(),
		...
    ];
}
```

_Last reivew date: Jul 9, 2018_

[//]: # (by Valeriy Pravoslavny)