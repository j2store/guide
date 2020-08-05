# Tranzila Payment Plugin

This plugin integrates Tranzila payment gateway with J2Store.

**Installation** You can install the plugin through the standard Joomla installer.

**Configuration** Before you set up the plugin, you need to configure your Tranzila system.

**Tranzila setup**

1. Login to your Tranzila testing / live account.
2. Setup the “Server IP” to match your machine IP, under the “Respond to a User Agent object including http headers”, and make sure that radio is checked.
3. We’ll add some keys that will allow us to send J2Store specific data, such as the order ID, the product description.
4. Goto Settings &gt;&gt; Config 2 &gt;&gt; Section 3 \(User Defined Fields\).
5. Under “Field name on Form” and “Field name on Screen” add:

order\_id \| Order ID description \| Description

**Plugin Set up** Go to Joomla admin → J2Store → Set up → Payment → Tranzila Payments → Edit

**Parameters** **Payment Option title** Enter a name that will be shown in the payment methodsselection during the checkout process. Default Tranzila

**Supplier ID** Your Tranzilla Supplied ID

**Tranzila System URL** Choose the Tranzila System url, which was provided to you. Thiswill normally be secure5.tranzila.com

**Joomla Article ID for custom thank you message** You can create an Article ID with a message enter its ID here to show it to the customer after completion of the purchase.

**Display Text on Selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below.

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display Text before Payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display Text after Payment/Order** The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display Text on Error in Payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display Text on Cancel Payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Testing Information** You may use a dummy number which simulates a Visa card number – 4444333322221111. The CVV should be any three digit number, for example - 333. Another dummy number to simulate Isracard is 12312312. Contact Tranzilla for more information on test credit cards.

**Troubleshooting** When submitting an order, J2Store may return an error about

> “Credit cart could not be processed…”

This might not necessarily mean it isn’t working.

You can check it in two places:

1. In the Tranzila account go to Transactions &gt;&gt; Today &gt;&gt; All, and see if your order was registered. If so, it means it worked ok on your settings are correct. The fact that it didn’t return “000” \(Payment accepted\) as a response. Perform some more test purchases. If the problem persists, contact the Tranzila Support.
2. If your order was not registered in your Tranzila, then it means wrong settings. Check your server IP and make sure your entered the IP correctly.

**Support** Still have questions? You can post your questions in our support forum: [http://j2store.org/forum/index.html](http://j2store.org/forum/index.html)

