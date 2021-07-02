# Redsys/Servired/Sermepa Payment Plugin

This plugin integrates the TPV RedSys / Servired / Sermepa payment system used by Spanish banks. It supports banks including - La Caixa, Banco Sabadell, Caixa Penedes, Caja Rural, Unnim, Deutsche Bank.

Full list can be read from here: [click here](http://www.servired.es/espanol/miembros.htm)

**Configuration Parameters**

**Payment option title** The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**Payment Page title** Title displayed in the payment page of TPV Redsys/servied / sermepa gateway. Add a Title, ex: “La Caixa”.

**Commerce number \(número de comercio\)\(FUC\)** The merchant commerce number provided by your bank

**Commerce signature \(secret\) key** A secret key provided by your bank / payment gateway

**Terminal Number \(número de terminal\)** The terminal number provided by your bank / the payment gateway

**Method of Encryption** Encryption standard. It would be either sha1-enhanced or sha. SHA1-Enhanced will be used by most of the banks. Read your Bank welcome documentation.

**Use Sandbox/test mode** Enable this to test your integration with the TPV Redsys / Servired /Sermepa test system. Your bank will provide the test credentials. First turn this on and test your integration. Once you are ready, contact with your Bank and once you are live, disable this.

**Customer Currency \(optional\)**

If a currency in your store is not supported by the gateway, Then the order will be converted to this currency automatically. Default is EURO.

**Customer language** The language of the payment screen displayed to the customer \(at the TPV Redsys / servired / sermepa end\)

**Transaction Type** The transaction type: It can be either Authorization orPre-Authorisation. I

> MPORTANT: Some banks will not allow pre-authorisation. So you have to make sure that your account can accept pre-authorisation transactions.

**Article ID for Thank you message:**

You can create an article with a thank you or instructions or information to the customer and enter its ID here. This will be displayed to the customer when he returns to the site after making payment

**Display Text on Selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below.

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display Text before Payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display Text after Payment/Order** The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display Text on Error in Payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display Text on Cancel Payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can entr a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment Button Text** The text of the payment button. The button will be displayed at the final checkout step.

**Support** Still have questions? You can post your questions in our support forum: [click here](http://j2store.org/forum/index.html)

