---
title: Install the [!DNL Express Checkout] for Adobe Commerce extension
description: Follow these steps to install the [!DNL Upgrade Compatibility Tool] for your Adobe Commerce project.
exl-id: e1dabc9a-0ab0-4f8d-98d3-7a32abbedcb8
---
# Install the [!DNL Express Checkout]

>[!IMPORTANT]
>
> This feature is for Early Adopter Program (EAP) users only and is not yet accessible for all customers. Currently limited to US customers. Contact Adobe Commerce Support for assistance and questions.

The [!DNL Express Checkout] for Adobe Commerce powers a seamless checkout experience designed to convert one-time guest shoppers into loyal account holders.

The [!DNL Express Checkout] extension for Adobe Commerce and Magento Open Source can be installed with Composer keys, which are linked to the [Magento ID (mageid)](https://devdocs.magento.com/marketplace/sellers/profile-personal.html#field-descriptions){target="_blank"} provided in the signup process. Composer uses these keys during the initial installation of Adobe Commerce, or in situations in which the Composer keys were not previously saved to the `auth.json` file.

See [get your authentication keys](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target="_blank"} for more information about obtaining Composer keys.

There are two ways to install this extension---for [Adobe Commerce on cloud infrastructure](#magento-commerce-cloud) or [on-premises](#on-premises) installations. These methods require you to use the Command Line Interface (CLI).

## Update minimum-stability setting

Before you install the extension, you can change the `minimum-stability` requirement to `RC` (release candidate) in your `composer.json` file if you want to try the release candidate version. You can use an IDE or your favorite text editor (like Visual Studio Code or Sublime Text).

In your `composer.json` file, change `"minimum-stability": "stable"` to `"minimum-stability": "RC"`.

## Install the extension

You can install the [!DNL Express Checkout] extension for both Adobe Commerce on cloud infrastructure and on-premises instances.

### Adobe Commerce on cloud infrastructure

This method is used for installing the [!DNL Express Checkout] extension for a Commerce Cloud instance.

1. On your local workstation, change to the Cloud project root directory.

1. Update your `composer.json` file:

   ```bash
   composer require magento/express-checkout --no-update
   ```

1. Update dependencies and install the extension:

   ```bash
   composer update
   ```

   The `composer update` command updates all dependencies. If you do not want to update all dependencies at the same time, use this command instead: `composer update magento/express-checkout`.

1. Commit and push your changes.

### On-premises

This method is used for installing the [!DNL Express Checkout] extension for an On-premises instance.

1. Add the Express Checkout module to the `require` section of the `composer.json` file:

   ```bash
   composer require magento/express-checkout --no-update
   ```

1. Update dependencies and install the extension:

   ```bash
   composer update
   ```

   The `composer update` command updates all dependencies. If you do not want to update all dependencies at the same time, use this command instead: `composer update magento/express-checkout`.

1. Upgrade Adobe Commerce:

   ```bash
   bin/magento setup:upgrade
   ```

1. Clear the cache:

   ```bash
   bin/magento cache:clean
   ```

1. Commit changes.
1. Update your on-premises instance to ensure the committed code is deployed.

## Upgrade the extension

When we release a new version of the [!DNL Express Checkout], you can easily upgrade your extension.

1. To obtain the most recent version of the package:

   ```bash
   composer update
   ```
   
   The `composer update` command updates all dependencies. If you do not want to update all dependencies at the same time, use this command instead: `composer update magento/express-checkout`.

1. Commit and push your changes.

## Troubleshooting

You may see errors when attempting to install the [!DNL Express Checkout] extension.

Refer to the [troubleshooting](../express-checkout/troubleshooting.md) topic for more information if you encounter any issues when you install the [!DNL Express Checkout].

## Prerequisites

See the [prerequisites](../express-checkout/prerequisites.md) topic for more information.
