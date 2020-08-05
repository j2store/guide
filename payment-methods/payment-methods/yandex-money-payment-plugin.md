# Yandex Money Payment Plugin

This plugin integrates J2Store with the Yandex Money payment gateway.

**Installation** Go to Extensions Manager and Install the plugin by choosing the plugin file.

**Configuration**

1. Go to Joomla admin → J2Store → Set up → Payments → Yandex Money.
2. Click Edit plugin params and Fill in the params \(refer the explanations below\) .
3. Save the plugin and enable it.

**Payment option title** Enter a name. This will be displayed in the Payment selection page on checkout.

**Account Type** Choose your Yandex Account type. Yandex offers two account types, Personal and Business.

**Parameters for Personal Account TypeYandex Purse** **Your Yandex Purse ID**

**Payment Methods**

You can choose two methods here:

1. Yandex Money
2. Credit Cards - VISA, MasterCard, Maestro

**Parameters to be filed in your Yandex Personal Account**

You will have to submit a technical form provided by Yandex when you open an account. In the form where it asks for HTTP Notifications URL \(paymentAvisoURL\), enter the url displayed here.

**Parameters for Yandex Business Account TypeShop ID** Shop id provided by Yandex

**SCID** Scid provided by Yandex

**Payment Methods \( Choose your methods \)**

1. Yandex Money
2. Credit Cards - VISA, MasterCard, Maestro
3. Cash on hands
4. Payment from the account of a Mobile Phone
5. Webmoney e-currency

**Parameters to be filed in your Yandex Business Account** You will have to submit a technical form provided by Yandex when you open an account. In the form where it asks for HTTP Notifications URL \(paymentAvisoURL\), Check URL, Success URL, fail URL, enter the values displayed here.

**Shop Password** Your shop password provided by Yandex.

**Use Yandex Sandbox** If you want to test your set up, set this to yes.

> IMPORTANT: This should be set to NO if your site is LIVE.

**Article ID for Thank you message:** You can create an article with a thank you or instructions or information to the customer and enter its ID here. This will be displayed to the customer when he returns to the site after making payment.

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

**Support** Still have questions? You can post your questions in our support forum: [http://j2store.org/forum/index.html](http://j2store.org/forum/index.html)

