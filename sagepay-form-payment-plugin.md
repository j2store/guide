# Sagepay Form Payment Plugin

This Plugin integrates with the SagePay using the Form API.

**Server Requirements**

1. PHP 5.2 or higher
2. Joomla 2.5.x
3. J2Store 2.0 or above

**SagePay Requirements**

1. Make sure both Billing and Shipping addresses are enabled. Because SagePay requires both these addresses.
2. In your MySagePay account, make sure you enter the IP address of your website. Otherwise, you would receive Invalid results.

**Installation Instructions**

1. Use the Joomla installer to install the plugin.
2. In the backend, go to Extensions-&gt;Plugin Manager and open the Sagepay Payments \(Form\) plugin. \(type=j2store\).
3. Enable the plugin
4. Enter the parameters \(read the explanation about each parameter given below\)
5. Save and close it.

Now you can see the Sagepay Payments as an option during the Checkout process.

**Parameters**

**Payment Option Title** Enter a title for this payment option. This will be shown to the customers at the checkout. Default: Sagepay payments \(Form\)

**Vendor Name** Vendor name provided by SagePay

**Encryption Key** Encryption Key provided by SagePay.

**Vendor Email \(s\) \(Optional\)** If provided, an email will be sent to this address when each transaction completes \(successfully or otherwise\).

NOTE: If you wish to use multiple email addresses, you should add them using the : \(colon\) character as a separator. e.g., e.g., me@mail1.com : me@mail2.com

**Use SagePay Sandbox** SagePay offers a testing suite. Before going live, you can test your store using the Sagepay test server.

IN LIVE SITE, THIS SHOULD BE SET TO NO.

**Article ID for Thanks you message** You can create an article to say thanks, provide some information or instructions to the customers, who purchased in your online store. Enter the Article ID here. This will show, when customers return from the paypal.

**Display Text on Selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below.

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display Text before Payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display Text after Payment/Order** The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display Text on Error in Payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display Text on Cancel Payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment Button Text** The text of the payment button. The button will be displayed at the final checkout step.

**Support** Still have questions? You can post your questions in our support forum: [click here](http://j2store.org/forum/index.html)

