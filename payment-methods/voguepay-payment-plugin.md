# Voguepay Payment Plugin

The Voguepay Plugin for J2Store enables you to receive payments via Voguepay Payment Gateway. This integrates the Voguepay’s Website Standard Payment API.

**Requirements**

1. PHP 5.2 or higher
2. Joomla 2.5.x
3. J2Store 2.0 or above

**Installation Instructions**

1. Use the Joomla installer to install the plugin.
2. In the backend, go to Extensions-&gt;Plugin Manager and open the Voguepay Payments plugin. \(type=j2store\).
3. Enable the plugin
4. Enter the parameters \(read the explanation about each parameter given below\)
5. Save and close it.

Now you can see the Voguepay Payments as an option during the Check out process.

**Parameters** **Voguepay Merchant ID**

This is your original Voguepay Merchant id, can be found on the top right hand side after you login in the Voguepay Site.To get site id and secure site code

1. Login into your Voguepay Account, If you don’t have an account then create an account.Go to the link:https://Voguepay.com”target = ¨\_blank”rel = ¨noopener¨&gt; click here
2. After Successfull login you will get Merchant ID \( Parameter: Voguepay Merchant ID\).Use Voguepay Test ModeVoguepay offers a test environment. Before going live, you can test your store using the Voguepay’s test environment.By setting this Test mode ON , your merchand ID will be set as demo.

> IN LIVE SITE, THIS SHOULD BE SET TO NO.

**Article ID for Thanks you message** You can create an article to say thanks, provide some information or instructions to the customers, who purchased in your online store. Enter the Article ID here. This will show, when customers return from the Voguepay.

**Geozone** By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.Logo Image for display in VoguepayThe URL of the 150x50-pixel image displayed as your logo in the upper left corner of Voguepay’s pages. Default: your business name \(if you have a Business account\) or your email address \(if you have Premier account\). If this is not working, try using the Custom Header Image param above.This is an optional setting.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips belowTip - ONLY FOR MULTI-LINGUAL SITESFor example, enter a language constant:J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order** The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process.You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on customers cancel payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\).You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.Payment Button TextThe text of the payment button. The button will be displayed at the final checkout step.

**Debug:** Set Yes to enable to debugging. NEVER AND EVER set this in Live site.

Relevant Screen Shot

![voguepay](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/voguepay-payment-plugin/paymenvoguepay.png)

This is Screen shot Will help you to Enable Test Mode, To test Your Store before going live.

**Support** Still have questions? Post in our support forum: [http://j2store.org/forum/index.html](http://j2store.org/forum/index.html)

Thank you for using our extension.

