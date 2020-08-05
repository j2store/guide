# Paybox Payment plugin

This plugin integrates Paybox Payment gateway with J2Store.

IMPORTANT NOTE: Most of the payment options provided by Paybox accept Euro as the currency. So make sure that you create EUR as one of the currencies in J2Store.

**System Requirements**

1. PHP 5.3
2. Joomla 2.5+
3. J2Store 2.6.7+

**Configuration**

The plugin has the following parameters need to be addressed.

**Payment option title** The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**Site Number \(PBX\_SITE\)** The site number provided by the Paybox

**Rank Number \(PBX\_R ANG\)** Rank number provided by Paybox

**Rank Number \(PBX\_IDENTIFIANT\)** Identifier provided by Paybox

**Secret key** A secret hash provided by Paybox. The value to put in this field can be found in the merchant back office in the information tab in the menu. For individual merchant accountsyou need to follow the procedure to generate your own secret key. For test account, the secret key is fixed and can be obtained from Paybox

**Public Key** A public encryption key provided in the form a certificate. You can download it from the paybox site. We have also attached the certificate downloaded from paybox. Open the file and copy its content to this field.

**Show other currencies in the payment page \(info only\)**

Set this to yes if you want to show other currencies in the Paybox payment page. Just the information only.

**Use Paybox Sandbox** Set this to Yes, if you want to test the integration with the Paybox pre-production/test server.

IMPORTANT: Never, ever, set this to Yes when your site is Live.

**Article ID for Thanks Message** You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.

**Refer the tips below**

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order** The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on cancel payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment Button Text** The text of the payment button. The button will be displayed at the final checkout step.

**Support** Still have questions? You can post in our supportforum:click here

Thank you for using our extension.

