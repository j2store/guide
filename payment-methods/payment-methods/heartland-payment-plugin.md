# Heartland Payment Plugin

This plugin integrates J2Store with Heartland Payment Gateway enabling you to accept credit cards.

## Requirements <a id="requirements"></a>

1. PHP 5.2 or higher
2. Joomla 2.5 or above
3. J2Store 2.7.3 or above

## Installation Instructions <a id="installation-instructions"></a>

1. Use the Joomla installer to install the plugin.
2. In the backend, go to Extensions-&gt;Plugin Manager and open the Heartland Payment plugin. \(type = j2store\).
3. Enable the plugin.
4. Enter the parameters \(read the explanation about each parameter given below\).
5. Save and close it.

## Parameters <a id="parameters"></a>

**Payment option title** Enter a title for this payment method. This text will be displayed while listing the payment methods during checkout. This is an optional parameter.

**API Key** This is your Heartland Account API Key.

**Version Number** This is your Heartland Account Version Number

**Developer ID** Heartland Account Developer ID

**Geo Zone** By selecting a Geozone here, you can restrict customers of a selected Geo-regions from viewing the payment method. Choose all Geozones to show the payment method to customers of all Geo-regions.

**Display text on selection** The text entered here is displayed when a customer selects this payment method. You can enter a language constant as a value here, if you are using a multi-lingual site and thenwrite a language override. Refer the tips below:

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all languages.

**Display text before payment** The text entered here is displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here, if you are using a multi-lingual site and then write a language override. Refer the Display text on selection param.

**Display text on error in payment** The text entered here is displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection param.

**Display text on after payment** The text entered here will be displayed to the customer on after payment in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site andthen write a language override. Refer the Display text on selection param.

**Debug Payment** This option used to enable/disable log file.

**Payment Button Text** The text of the payment button. The button will be displayed at the final checkout step.

**Support** Still have questions? You can reach us in [click here](http://j2store.org/forum/index.html)

Thank you for using our extension.

