---
title: Legacy Payment Services configuration
description: After installation, you can configure [!DNL Payment Services] in the Admin at the store configuration.
role: Admin, User
level: Intermediate
exl-id: e1a3269d-bdf9-4b0f-972f-e8a0ef469503
---
# Legacy Payment Services configuration

You can customize [!DNL Payment Services] to your needs with helpful configuration options in the Admin.

When you configure [!DNL Payment Services] for Adobe Commerce and Magento Open Source in the Admin, those configurations apply only to the environment that is set in the [!UICONTROL Method] field of [!UICONTROL General Configuration]. Any changes you make in the configuration fields are independent of switching the [!UICONTROL Method] selection---if you switch the method, your selections do not reset.

See the [[!UICONTROL General Configuration] section](#general-configuration) for more information.

## General configuration

You can enable [!DNL Payment Services] for your store, and enable either sandbox testing or live payments in the [!UICONTROL General Configuration] section.

1. On the _Admin_ sidebar, go to **[!UICONTROL Stores]** > _[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**.
1. In the left panel, expand **[!UICONTROL Sales]** and choose **[!UICONTROL Payment Methods]**.

   ![Methods view](assets/methods-view.png)

1. Expand the _[!UICONTROL Recommended Solutions]_ section.
1. In the _[!UICONTROL [!DNL Payment Services]]_ section, expand the _[!UICONTROL General Configuration]_ section.
1. For **Enable**, set it to `Yes` to enable [!DNL Payment Services] for your store.
1. For **Method**, set it to `Sandbox` if you are still testing [!DNL Payment Services] for your store or `Production` if you are ready to enable live payments.

   >[!WARNING]
   >
   >Your [!UICONTROL Sandbox Merchant ID] and [!UICONTROL Production Merchant ID] are auto-generated and present in their respectable fields when you have finished onboarding for the sandbox and/or production. Do not remove or change these IDs.

1. Click **[!UICONTROL Save Config]** to save your changes.

### Configuration options

| Field | Scope | Description |
|---|---|---|
| [!UICONTROL Enable] | website | Enable or disable [!DNL Payment Services] for your website. Options: [!UICONTROL Yes] / [!UICONTROL No] |
| [!UICONTROL Method] | store view | Set the method, or environment, for your store. Options: [!UICONTROL Sandbox] / [!UICONTROL Production] |
| [!UICONTROL Sandbox Merchant ID] | store view | Your sandbox merchant ID, which is auto-generated during sandbox onboarding. Do not change or alter this ID. |
| [!UICONTROL Production Merchant ID] | store view | Your production merchant ID, which is auto-generated during sandbox onboarding. Do not change or alter this ID. |

## [!UICONTROL Credit Card Fields]

The [!UICONTROL Credit Card Fields] payment options provide a simple and secure checkout for credit card or debit card payment methods.

See [Payments options](payments-options.md#paypal-smart-buttons) for more information.

### Configure Credit Card Fields

1. On the _Admin_ sidebar, go to **[!UICONTROL Stores]** > _[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**.
1. In the left panel, expand **[!UICONTROL Sales]** and choose **[!UICONTROL Payment Methods]**.
1. Expand the _[!UICONTROL Recommended Solutions]_ section.
1. In the _[!UICONTROL Payment Services]_ section, expand the _[!UICONTROL Credit Card Fields]_ section.
1. For **[!UICONTROL Title]**, enter text (if needed) to change the name of the payment method as shown during checkout.
1. To [set the payment action](production.md#set-payment-services-as-payment-method), select **[!UICONTROL Authorize]** or **Authorize and Capture**.
1. For **Debug Mode**, choose `Yes` to enable debug mode (or `No` to disable it).
1. Click **[!UICONTROL Save Config]** to save your changes.

#### Configuration options

| Field | Scope | Description |
|---|---|---|
| [!UICONTROL Title] | store view | Add the text for display as the title for this payment option in the Payment Method view during checkout. Options: [!UICONTROL text field] |
| [!UICONTROL Payment Action] | website | The [payment action](https://docs.magento.com/user-guide/configuration/sales/payment-methods.html#payment-actions){target="_blank"} for the specified payment method. Options: [!UICONTROL Authorize] / [!UICONTROL Authorize and Capture] |
| [!UICONTROL Debug Mode] | website | Enable or disable Debug Mode. Options: [!UICONTROL Yes] / [!UICONTROL No] |

## [!DNL PayPal Smart Buttons]

The [!DNL PayPal Smart Buttons] payment options provide a simple, fast, and secure checkout process for your customer.

See [Payments options](payments-options.md#paypal-smart-buttons) for more information.

### Configure [!DNL PayPal Smart Buttons]

You can enable and configure the PayPal Smart Buttons payment options within the Admin:

1. On the _Admin_ sidebar, go to **[!UICONTROL Stores]** > _[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**.
1. In the left panel, expand **[!UICONTROL Sales]** and choose **[!UICONTROL Payment Methods]**.
1. Expand the _[!UICONTROL Recommended Solutions]_ section.
1. In the _[!UICONTROL Payment Services]_ section, expand the _[!UICONTROL PayPal Smart Buttons]_ section.
1. To change the name of the payment method as shown during checkout, edit the _[!UICONTROL Title]_ field.
1. To [set the payment action](production.md#set-payment-services-as-payment-method), select **[!UICONTROL Authorize]** or **[!UICONTROL Authorize and Capture]**.
1. To disable the [Pay Later messaging](payments-options.md#pay-later-button) (if desired), select `No` for **[!UICONTROL Display Pay Later Message]**.
1. To enable debug mode, select `Yes` for the **[!UICONTROL Debug Mode]** (`No` disables it).
1. To save your changes, click **[!UICONTROL Save Config]** .

### Configuration options

| Field | Scope | Description |
|---|---|---|
| [!UICONTROL Title] | store view | Add the text to be displayed as the title for this payment option in the Payment Method view during checkout. Options: text field |
| [!UICONTROL Payment Action] | website | The [payment action](https://docs.magento.com/user-guide/configuration/sales/payment-methods.html#payment-actions){target="_blank"} for the specified payment method. Options: [!UICONTROL Authorize] / [!UICONTROL Authorize and Capture] |
| [!UICONTROL Display Pay Later Message] | website | Enable or disable the Pay Later messaging in the shopping cart, product page, mini-cart, and during the checkout flow. Options: [!UICONTROL Yes] / [!UICONTROL No] |
| [!UICONTROL Venmo Enabled] | store view | Enable or disable venmo payment option where payment buttons are displayed. Options: [!UICONTROL Yes] / [!UICONTROL No] |
| [!UICONTROL PayPal Pay Later Enabled] | store view | Enable or disable pay later payment option appearance where payment buttons are displayed. Options: [!UICONTROL Yes] / [!UICONTROL No] |
| [!UICONTROL Debug Mode] | website | Enable or disable Debug Mode. Options: [!UICONTROL Yes] / [!UICONTROL No] |
| [!UICONTROL Show buttons on product detail page] | store view | Enable or disable [!DNL PayPal Smart Buttons] on the product detail page. Options: [!UICONTROL Yes] / [!UICONTROL No] |
| [!UICONTROL Show buttons in mini cart preview] | store view | Enable or disable [!DNL PayPal Smart Buttons] in the minicart preview. Options: [!UICONTROL Yes] / [!UICONTROL No] |
| [!UICONTROL Show buttons on cart page] | store view | Enable or disable [!DNL PayPal Smart Buttons] on the cart page. Options: [!UICONTROL Yes] / [!UICONTROL No] |

### [!DNL PayPal Smart Buttons] Styling options

|Field|[Scope]({% link configuration/scope.md %})|Description|
|--- |--- |--- |
|[!UICONTROL Layout]|Store View|Define style of layout for Paypal Smart Buttons. Options: [!UICONTROL Vertical] / [!UICONTROL Horizontal]|
|[!UICONTROL Color]|Store View|Define color of the Paypal Smart Buttons. Options: [!UICONTROL Blue] / [!UICONTROL Gold] / [!UICONTROL Silver] / [!UICONTROL White] / [!UICONTROL Black]|
|[!UICONTROL Shape]|Store View|Define shape of the Paypal Smart Buttons. Options: [!UICONTROL Rectangular] / [!UICONTROL Pill]|
|[!UICONTROL Use Default Height]|Store View|Defines if PayPal Smart Buttons use a default height. Options: [!UICONTROL Yes] / [!UICONTROL No]|
|[!UICONTROL Height]|Store View|Define height of the PayPal Smart Buttons. Default value: none|
|[!UICONTROL Label]|Store View|Define label that appears in the PayPal Smart Buttons. Options: [!UICONTROL PayPal] / [!UICONTROL Checkout] / [!UICONTROL Buynow] / [!UICONTROL Pay] / [!UICONTROL Installment]|
|[!UICONTROL Tagline]|Store View|Enables tagline. Options: [!UICONTROL Yes] / [!UICONTROL No]|
