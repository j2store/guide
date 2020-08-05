# Direcpay Payment Plugin

This plugin integrates DirecPay payment gateway with J2Store.

## Installation <a id="installation"></a>

You can install the plugin through the standard Joomla installer.

## Configuration <a id="configuration"></a>

**Payment Option title** The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**Merchant ID** The merchant ID provided by DirecPay.

Note: DirecPay provides a separate merchant ID for testing. For Live transaction, the merchant ID differs.

**Encryption Key** A secret encryption key provided by the DirecPay.

**Use Sandbox** Set yes to test the integration of the plugin with the DirecPay test server.

**Article ID for Thank you message** You can create an article with a thank you or instructions or information to the customer and enter its ID here. This will be displayed to the customer when he returns to the site after making payment.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order** The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on cancel payment**

The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment Button Text** The text of the payment button. The button will be displayed at the final checkout step.

**Support**

Still have questions? You can post in our supportforum: [click here](http://j2store.org/forum/index.html)

Thank you for using our extension.

