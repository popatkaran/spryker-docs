---
title: Company Account- Reference Information
description: The guide provides additional information on the values you use when working with company roles, company unit addresses, company units, and company users.
originalLink: https://documentation.spryker.com/v2/docs/company-account-reference-information
originalArticleId: 4bbf063a-4bf0-4d57-8f88-9a142b1bdea6
redirect_from:
  - /v2/docs/company-account-reference-information
  - /v2/docs/en/company-account-reference-information
---

This article describes the information that you may need to know when working with the company account setup.
***
The following table describes the information that you see on the overview pages of the **Company Account** section.

| Page Name | Information |
| --- | --- |
| **Overview of Company Users** | You see the user ID, the company name to which the user is assigned the user name, roles assigned to the user, company business unit to which the user is assigned, status of the user and the actions that you can perform (**Edit**, **Disable**, **Delete**, **Attach to BU**) |
| **Overview of Company Business Units**|You see the autogenerated ID, your company name, business unit parent and the business unit name, address of headquarters business unit, IBAN and BIC, the list of actions that you can do (**Edit**, **Delete**). |
| **Overview of Companies** | You see the company ID and name, either Active, or Inactive label, the company status (either **Approved** or **Declined**), and the actions you can perform (**Edit**, **Activate**/**Deactivate**, **Approve**/**Deny**).  |
| **Overview of Company Roles** | You see the role ID, the name of the company to which the role is assigned, role name, and the actions that you can perform (**Edit**, **Delete**). |
| **Overview of Business Unit Addresses** | You see the company unit address ID, country, city, zip code, company name, address, number, addition to address, any labels if those are assigned and the actions that you can perform (**Edit Company Unit Address**). |
***
## Create/Edit Company User
The following table describes the attributes you see, select, or enter while creating or editing a company user.
| Attribute |Description  |
| --- | --- |
| **Email** | The email of the customer that is used for logging in to the online store. It is not available for modifications on the **Edit** page. |
| **Salutation** | Formal salutation for the customer (_Mr_, _Mrs_, _Ms_, _Dr_). |
| **First Name** | Customer first name. |
| **Last Name** |  Customer last name.|
| **Gender** | Customer gender. |
| **Date of birth** | Customer date of birth. |
|**Company**  | A drop-down list with the companies from the Company Account > Companies section. This selection defines the list of available business unit. |
| **Business Unit** | Business unit to which the user is going to be assigned. The list of the available values depends on the selected company. |
| **Assigned Roles** | The roles assigned to the customer. |
|**Unassigned Roles**|The roles that you can select to be assigned to the customer.|
***
## Create/Edit Company Business Unit
The following table describes the attributes you see, select, or enter while creating or editing a company business unit.
| Attribute |Description  |
| --- | --- |
| **Company** | A drop-down list with the companies. On the **Create** page, all companies form the **Companies** section are available for selection. On the **Edit** page, the filed is a display only. The company selected during the business unit creation cannot be changed. |
| **Parent** | The parent business unit. The values available for selection depend on the selected companies. |
| **Name** | The name of the business unit you create.|
| **IBAN** |  The International Bank Account Number. |
|**BIC**  | The Bank Identifier Code. |
| **Addresses** |This field is available on the Edit page. This is a multi-select list that includes the values from the Company Unit Addresses section but only those assigned to a company. Meaning the values available for selection are defined by the selected company.| 
***
## Create/Edit Company Unit Address
The following table describes the attributes you see, select, or enter while creating or editing a company unit address.

| Attribute | Description |
| --- | --- |
| **Company** | A drop-down list with the values from the **Company Account > Company** section. |
| **Country** | A drop-down list with the countries available for selection. |
| **City** | A text field where you enter the city name. |
| **Zip Code** | A text field where you enter zip code value. |
| **Street** | A text field where you enter the street name. |
| **Number** | A text field where you enter the street number. |
|**Addition to address**|A text field where you enter any additions to the address that you create.|
|**Comment**|A text field where you enter any comment regarding the customer address.|
|**Labels**| A multi-select field with the labels for selection.|
***

**Examples**
**Company User Profile**
| Back Office: Company User Record | Online Store: Company User Profile |
| --- | --- |
| ![Back Office: Company User Profile](https://spryker.s3.eu-central-1.amazonaws.com/docs/User+Guides/Back+Office+User+Guides/Company+Account/Company+Account:+Reference+Information/company-user-profile-backoffice.png)  | ![Online Store: Company User Profile](https://spryker.s3.eu-central-1.amazonaws.com/docs/User+Guides/Back+Office+User+Guides/Company+Account/Company+Account:+Reference+Information/company-user-profile-online-store.png)  |

**Company Roles**

| Back Office: Company Roles | Online Store: Company Roles |
| --- | --- |
| ![Back Office: Company Role](https://spryker.s3.eu-central-1.amazonaws.com/docs/User+Guides/Back+Office+User+Guides/Company+Account/Company+Account:+Reference+Information/company-role-backoffice.png)  | ![Online Store: Company Role](https://spryker.s3.eu-central-1.amazonaws.com/docs/User+Guides/Back+Office+User+Guides/Company+Account/Company+Account:+Reference+Information/company-role-online-store.png)  |

**Company Users**

| Back Office: Company Users |Online Store: Company Users |
| --- | --- |
| ![Back Office: Company User](https://spryker.s3.eu-central-1.amazonaws.com/docs/User+Guides/Back+Office+User+Guides/Company+Account/Company+Account:+Reference+Information/company-user-backoffice.png)  | ![Online Store: Company User](https://spryker.s3.eu-central-1.amazonaws.com/docs/User+Guides/Back+Office+User+Guides/Company+Account/Company+Account:+Reference+Information/company-user-online-store.png)  |