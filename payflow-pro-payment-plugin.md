# Payflow Pro Payment plugin

This plugin integrates the Payflow PRO gateway with J2Store. Accepted cards include Visa, MasterCard, Switch/Maestro, and Solo credit cards in the United States.

Payflow PRO is available only for merchants in US, Canada, Australia, New Zealand.

**Requirements**

1. PHP 5.3 or higher
2. Joomla 2.5.x
3. J2Store 2.6.3

**Installation Instructions** Use the Joomla installer to install the plugin like you do for other extensions.

**Configuring the Plugin** Go to Joomla admin → Extensions → Plugin Manager → Paypal Payflow PRO.

**Payment option title** The value entered here will be used as the title for this payment method. Customer will see this value when he checks out. Default: Payflow PRO

**Vendor/Merchant Login** The Merchant Login with which you login to Paypal Manager

**User** Your User ID. If you created a new user, then enter that user id here. If not, then this field should carry the same value as the Vendor/Merchant Login.

**Password** Your password with which you login to Paypal manager

PartnerYour PayPal partner ID. By default, it will be PayPal.

**Transaction Type** The type of transaction. If you choose SALE, then the payment will be captured immediately after a customer makes the payment. If you choose Authorization, then Payment will not be captured. You will have to capture it manually by going to Paypal Manager. Default value: Sale

**Use sandbox for testing** Set this to YES, only if your account is in TEST mode.

IN LIVE SITE, THIS SHOULD BE SET TO NO.

**Article ID for Thank you message** You can create an article with a thank you or instructions or information to the customer and enter its ID here. This will be displayed to the customer when he returns to the site after making payment.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order** The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on cancel payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment Button Text** The text of the payment button. The button will be displayed at the final checkout step.

**Support** Still have questions? You can post your questions in our support forum: [click here](http://j2store.org/forum/index.html) Thank you for using our extension.

