# Braintree payment plugin

This plugin integrates Braintree payment gateway with J2Store.

You need an account with Braintree to choose this method. If you have/create one, you will be provided with Merchant Id,private and public keys for facilitating payments. You need to enter them in the respective fields. In these payment types, unlike Bank Transfer or Money order methods, the customer has the option to cancel the payment. Also, if any error occurs during payment process, that will be logged. These will be notified through the additional text boxes provided.

## Installation <a id="installation"></a>

You can install the plugin through the standard Joomla installer.

## Configuration <a id="configuration"></a>

**Payment Option title**

Enter a name that will be shown in the payment methods selection during the checkout process. Default Braintree.

**Plugin Display Image :**

Select the image of the plugin that you wish display at the front end.

![plugin](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/braintree-payment-plugin/braintree-plugin.png)

**Live Merchant id :**

Enter your live account’s Merchant Id Key.

**Live Private Key**

Enter your live account’s Private API Key.

**Live Public Key**

Enter your live account’s Public API Key

**Test Merchant Account list**

The merchant details will be displayed after entering the Merchant key,public key,private key and clicking on save.

**Use sandbox**

This option allows you to test the plugin with Paymill in test mode instead of the live one.

IMPORTANT: NEVER ever set this to yes when your shop is live.

**Test Private Key**

Enter your test Private API Key here.

**Test Public Key**

This is the test public key to be used while testing the payment plugin. You can find these keys under your account settings.

**Test Merchant Account list**

The merchant details will be displayed after entering the Test merchant key, Test public key,Test private key and clicking on save

**Payment Type**

Choose the desired payment type according to the requirement.

 

![payment](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/braintree-payment-plugin/bt-payment-method.png)

**Display text on selection**

The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment**

The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order**

The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment**

The text entered here will be displayed to the customer when there is an error in the payment process.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on cancel payment**

The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\).

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment Button Text**

The text of the payment button. The button will be displayed at the final checkout step.

**Debug Mode:** Setting debug mode to yes will allow the errors to be logged in case of transaction failures.

**Support** Still have questions? You can post your questions in our support forum &lt;link-text url =":http://j2store.org/forum/index.html”target = ¨\_blank”rel = ¨noopener¨&gt; click here

Thank you for using our extension.

