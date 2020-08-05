# Payfast Payment plugin

This plugin integrates PayFast payment gateway with J2Store.

**Installation** You can install the plugin through the standard Joomla installer.

**Configuration**

**Payment Option title** Enter a name that will be shown in the payment methods selection during the checkout process. Default - Payfast

**Merchant ID** Your PayFast Merchant ID

**Merchant Key** The Merchant Key provided by PayFast

**Pass Phrase \(Md5 Secret\)** The secret word set up in your Payfast Merchant Account. To set up the secret word please log in to your Payfast account and click the EDIT button under Settings → Salt Pass Pharse.

**Surcharge percentage** This is an optional field. Use this field if you require. Otherwise leave it empty. If you want to charge a percentage of Total Order Value as additional fee to the customers who choose this payment method, then you can enter the fee here. Enter only a numeric value. DO NOT enter % or any other symbols.

**Surcharge Fixed** This is optional field. Use this field if you require. Otherwise leave empty. If you want to charge a Fixed amount as additional fee to the customers who choose this payment method, then you can enter the fee here. Enter only a numeric value. DO NOT enter % or any other symbols.

**Order Description** You can enter a text here, which will be sent as a description for the order.

**Use Sandbox** Setting this yes will make the plugin to use the Payfast sandbox server.

NEVER EVER set this to YES, when your site is live.

**Enable Payfast Email Notifications** Set this to Yes, if you want Payfast to send you notifications after a customer makes payment.

**Restrict this payment method to selected geozones** Leave this to All geozones if you dont know what you are doing.If you want to restrict showing Payfast only to a region, then you can create a geozone and choose it here. Customers from that region alone will see the Payfast as payment methodin the checkout steps.

**Article ID for custom thank you message** You can create an Article ID with a message enter its ID here to show it to the customer after completion of the purchase.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order** The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on cancel payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Support** Still have questions? You can post in our supportforum: [click here](http://j2store.org/forum/index.html)

