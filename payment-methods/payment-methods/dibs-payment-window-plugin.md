# DIBS Payment Window Plugin

The plugin integrates with the DIBS Payment Window method. Refer this page for more information.http://www.dibspayment.com/dibs-payment-window” traget = “\_blank”rel =“noopener”&gt; click here

## Requirements <a id="requirements"></a>

1. PHP 5.2 or higher
2. Joomla 2.5.x
3. J2Store 2.0.2 or above

## Installation Instructions <a id="installation-instructions"></a>

1. Use the Joomla installer to install the plugin.
2. In the backend, go to Extensions-&gt;Plugin Manager and open the DIBS Payment Window plugin\(type = j2store\).
3. Enable the plugin
4. Enter the parameters \(read the explanation about each parameter given below\)
5. Save and close it.

Now you can see the DIBS Payment Window as an option during the Check out process.

## Configuration <a id="configuration"></a>

The plugin has the following parameters need to be addressed:

**Payment option title** The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**DIBS Merchant ID** The Unique Merchant ID number provided by the DIBS

**Use Test mode** For testing purposes, set this parameter to Yes. Important: IT SHOULD BE SET TO “NO” IN LIVE SYSTEMS.

**Thanks Message Joomla Article ID** You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.

Refer the tips below Tip - ONLY FOR MULTI-LINGUAL SITES For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order** The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on cancel payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment Button Text** The text of the payment button. The button will be displayed at the final checkout step.

**Support** Still have questions? You can post in our supportforum: [click here](http://j2store.org/forum/index.html)

Thank you for using our extension.

