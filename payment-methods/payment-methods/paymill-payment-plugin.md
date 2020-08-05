# Paymill Payment plugin

This plugin integrates Paymill payment gateway with J2Store.

You need an account with Paymill to choose this method. If you have/create one, you will be provided with private and public keys for facilitating payments. You need to enter them in the respective fields.

![paymill1](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/paymill-payment/pay_paymill1.png)

In these payment types, unlike Bank Transfer or Money order methods, the customer has the option to cancel the payment. Also, if any error occurs during payment process, that will be logged. These will be notified through the additional text boxes provided. Check the image below.

![paymill2](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/paymill-payment/pay_paymill2.png)

## Installation <a id="installation"></a>

You can install the plugin through the standard Joomla installer.

## Configuration <a id="configuration"></a>

**Payment Option title** Enter a name that will be shown in the payment methodsselection during the checkout process. Default Paymill

**Live Private Key** Enter your live account’s Private API Key.

**Live Public Key** Enter your live account’s Public API Key

**Test mode** This option allows you to test the plugin with Paymill in test mode instead of the live one.

IMPORTANT: NEVER ever set this to yes when your shop is live.

**Test Private Key** Enter your test Private API Key here.

**Test Public Key** This is the test public key to be used while testing the shop. You can find these keys under your account settings.

**Article ID for Thank you message** You can create an article with a thank you or instructions or information to the customer and enter its ID here. This will be displayed to the customer when he returns to the site after making payment.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION. Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order** The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on cancel payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment Button Text** The text of the payment button. The button will be displayed at the final checkout step.

**Support** Still have questions? You can post your questions in our support forum: [click here](http://j2store.org/forum/index.html)

Thank you for using our extension.

