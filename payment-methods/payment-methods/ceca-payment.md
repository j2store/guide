# CECA Payment

This plugin integrates CECA payment gateway with J2Store Joomla eCommerce solution.

**Note:**

Euro\(EUR\) Currency Must be available in your store’s currency list.

Must set IPN url \(URL online OK:\) in CECA payment dashboard.

Online communication ok:\(Comunicación on-line OK:\) set to Yes \(SI\)

Answer required ok:\(Respuesta requerida OK:\) set to Yes \(SI\)

## Requirements <a id="requirements"></a>

* PHP version 5.4 +
* Joomla 3.x +
* J2Store 3.x +

## Installation <a id="installation"></a>

1. Download CECA Payment plugin from our site and install it using Joomla installer.
2. After installing the plugin, go to J2Store &gt; Setup &gt; Payment methods.
3. Enable CECA payment gateway for J2Store.
4. Now open the plugin and configure the basic settings of the app.

**Where to find the Merchant ID, Encryption key, Acquirer BIN, Terminal ID ?**

1. Log into your account through the address [click here](https://comercios.ceca.es/)
2. Enter your User number and password, you get the following screen
3. You can switch between real and testing environment on top left box. If you would like to use testing environment, click on Cambiar a datos de pruebas \(change to test data\) and the page will change from a blue to red which indicates that we are in a test environment.

![ceca](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/ceca-payment/ceca-switch-envi.png)

1. Once switched to testing environment, you will have to configure to get the data required. Click on Configuration.

![config](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/ceca-payment/ceca-config.png)

1. Once we are in configuration page, you can get all the following required data
2. Merchant ID
3. Acquirer BIN
4. Terminal ID
5. Encryption key

![ceca data](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/ceca-payment/ceca-req-data.png)

1. Now you must enter the following data in the configuration.Must set IPN url \(URL online OK:\) in CECA payment dashboard.Online communication ok:\(Comunicación on-line OK:\) set to Yes \(SI\)Answer required ok:\(Respuesta requerida OK:\) set to Yes \(SI\)

**Comunicación on-line OK: SI**

\(you can check this url in our plugin’s settings page\)

**Respuesta requerida OK: SI**

![cecaonline](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/ceca-payment/ceca-url-online.png)

1. Save.

**Use below test card details for testing purpose**

Test Card Number: 5020080001000006 Expiration date: \(December of current year\) CVV2: 989

## Payment plugin Configuration <a id="payment-plugin-configuration"></a>

**Payment option title** The value entered here will be used as the title for the payment. Customer will see this value when he checks out.

**Plugin display image** This image will be displayed while payment options are listed in the checkout page.

**IPN URL** Copy the url given here and paste it in payment configuration page [click here](https://comercios.ceca.es/)

**Merchant ID** Enter the merchant ID associated with live CECA account.

**Encryption key** Enter the Encryption key associated with live CECA account.

**Acquirer BIN** Enter the Acquirer BIN associated with live CECA account.

**Terminal ID** Enter the Terminal ID associated with live CECA account.

**Production url** If your payment have different product url, enter the url here. Otherwise leave it.

**Sandbox url** If your payment have different sandbox url, enter the url here. Otherwise leave it.

**Use Sandbox / test mode** CECA payment also offers sandbox feature to test your store. Select YES to use the payment in test mode.

**Sandbox Merchant ID** Enter the sandbox merchant ID associated with live CECA account.

**Sandbox Encryption key** Enter the sandbox Encryption key associated with live CECA account.

**Sandbox Acquirer BIN** Enter the sandbox Acquirer BIN associated with live CECA account.

**Sandbox Terminal ID** Enter the sandbox Terminal ID associated with live CECA account.

**Article ID for Thank You message** You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

**Geozone** By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on after payment** The text entered here will be displayed when customer completes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text if customers cancels payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment button text** Text entered here will be added as the name of the payment button. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.

**Debug** Choose YES to enable the debug mode. If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory. DO NOT select YES in the live site.

 

![payment](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/ceca-payment/ceca-payment-01.png)

![pay](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/ceca-payment/ceca-payment-02.png)

