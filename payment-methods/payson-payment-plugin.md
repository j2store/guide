# Payson Payment Plugin

This plugin integrates the Payson Payment gateway with J2Store.

**Installation** Use the Joomla extensions installer to install the plugin.

**Plugin Configuration** Go to Joomla admin → Plugin Manager and open the Payson plugin.

The plugin has following options:

**Payment option title** The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**Agent ID \(API ID\)** The API User ID \(Agent ID\) provided by Payson.

**MD5 Secret \(API Key\)** MD5 Secret \(API Key\) Provided by the Payson.

**Receiver email** This is your email that you have registered with Payson while opening an account.

**Test mode** Set this to YES if you want to test the plugin with the Test server of Payson.

Never set this to YES, when your site is live.

**Show Receipt** If you set this to Yes, payson will show a receipt to the customer after they made the payment and then returned to your site.

**Choose payment methods** Payson offers Credit card and bank payments. You can choose both or either one.

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

**Support** Still have questions? You can post your questions in our support forum: [click here](http://j2store.org/forum/index.html)

