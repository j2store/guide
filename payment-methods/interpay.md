# Interpay

This plugin implements Interac online web re-director which offers you privacy and security.

## System Requirements <a id="system-requirements"></a>

* PHP 5.4 or greater
* Joomla 3.x
* J2Store 3.2.x or greater

## Installation Instructions <a id="installation-instructions"></a>

1. Use the Joomla installer to install the plugin.
2. In the backend, go to J2store Dashboard Setup -&gt; Payment methods and enable InterPay Web Redirect for J2Store plugin.
3. Open the plugin and enter the parameters \(read the explanation about each parameter given below\)
4. Save and close it.

## Configuration <a id="configuration"></a>

**Payment option title** The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**Plugin Display Image** This image will be displayed while payment options are listed in the checkout page.

**TERMID** Enter the Term ID associated with your InterPay live account.

**PASS** Enter the “pass” associated with your InterPay live account.

**Test mode** InterPay payment offers you the sandbox feature. Before going live, you can test your store with this feature.

**Test TERMID** Enter the Term ID associated with your InterPay test account.

![interpay](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/interpay/interpay-01.png)

**Test PASS** Enter the “Pass” associated with your InterPay test account.

**Article Id for Thank you message** You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

**Geozone** By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

![itrpy](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/interpay/interpay-02.png)

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.

**Display text on after payment** The text entered here will be displayed when customer completes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment button text** Text entered here will be added as the name of the payment button. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.

**Debug** Choose YES to enable the debug mode. If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory. DO NOT select YES in the live site.

![intpay](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/interpay/interpay-03.png)

**Support** Still have questions? You can post in our support forum: [click here](http://j2store.org/forum/index.html)

Thank you for using our extension.

