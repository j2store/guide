# Checkout fi¨

This plugin integrates Checkout payment Finland with J2store.

## System Requirements <a id="system-requirements"></a>

* PHP 5.4 or greater
* Joomla 3.x
* J2Store 3.2.x or greater

## Installation Instructions <a id="installation-instructions"></a>

1. Use the Joomla installer to install the plugin.
2. In the backend, go to J2store Dashboard -&gt; Payment methods and enable plugin.
3. Open the plugin and enter the parameters \(read the explanation about each parameter given below\)
4. Save and close it.

## Configuration <a id="configuration"></a>

The plugin has the following parameters need to be addressed.

**Payment option title** The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**Plugin Display Image** This image will be displayed while payment options are listed in the checkout page.

**Merchant Id** This is your merchant ID provided by Payment Checkout Finland.

**Security Key** Enter your security key provided by Payment Checkout Finland.

**Use Sandbox** Payment Checkout Finland offers a testing suite called Sandbox. Before going live, you can test your store using this payment’s sandbox feature.

**Sandbox Merchant Id** Use your Payment Checkout Finland’s Sandbox merchant ID.

![checkout](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/checkout-fi/checkout_payment_finlandone.png)

**Sandbox security key** Use your Payment Checkout Finland’s Sandbox security key.

**Article id for thank you message** You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

**Geozone** By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on after payment** The text entered here will be displayed when customer completes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

![checkoutpayt](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/checkout-fi/checkout_payment_finlandtwo.png)

**Display text if customers cancels payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Debug** Choose YES to enable the debug mode. If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory. DO NOT select YES in the live site.

**Payment button text** Text entered here will be added as the name of the payment button. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.  
 

![checkpay](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/checkout-fi/checkout_payment_finlandthree.png)

**Support** Still have questions? You can post in our support forum: [click here](http://j2store.org/forum/index.html)

Thank you for using our extension.

