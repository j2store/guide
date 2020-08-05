# RealEx Payment Plugin

The plugin integrates RealEx payment gateway with J2Store Joomla eCommerce solution. RealEx is a popular European payment service providing secure credit card payment processing solutions.

**System Requirements**

1. PHP 5.4 or greater
2. Joomla 3.x
3. J2Store 3.2.x or greater

**Installation Instructions**

* Use the Joomla installer to install the plugin.
* In the backend, go to J2store Dashboard -&gt; Payment methods and enable plugin.
* Open the plugin and enter the parameters \(read the explanation about each parameter given below\)
* Save and close it.

**Configuration**

The plugin has the following parameters need to be addressed.

**Payment option title** The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**Plugin Display Image** This image will be displayed while payment options are listed in the checkout page.

**Payment Type**

> Choose your payment type

* Redirect method: Payment transaction will be processed in payment’s domain.
* Direct method: Payment transaction will be processed in J2store itself.

**Merchant Id** This is your merchant ID associated with RealEx payment.

**Account Id** Account ID entered here should be assoicated with RealEx payment.

**Secret Key** Secret key entered here should be associated with your RealEx payment account.

**Card Type** RealEx payment accepts VISA, MASTERCARD, CB, DINERS, AMERICAN EXPRESS, JCB card types. Please choose your card type from the list.

**Use Realex Sandbox** Choose YES to use RealEx payment’s sandbox feature.

**Test Merchant Id** Enter your RealEx payment’s sandbox Merchant ID.

**Test Account Id** Enter your RealEx payment’s sandbox Account ID.

Test Secret KeyEnter your RealEx payment’s sandbox secret key.

**Geozone** By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.

**Article Id for Thank you message** You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on after payment** The text entered here will be displayed when customer completes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text if customers cancels payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment button text** Text entered here will be added as the name of the payment button. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.

**Debug** Choose YES to enable the debug mode. If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory. DO NOT select YES in the live site.

**Support** Still have questions? You can post in our support forum: [click here](http://j2store.org/forum/index.html)

Thank you for using our extension.

