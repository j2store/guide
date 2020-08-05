# Culqi Payment

This plugin integrates a secure payment gateway Culqi with J2Store. This allows users of the store to pay via Culqi. This payment gateway accept credit and debit cards for payment on your store.

## Requirements <a id="requirements"></a>

1. PHP version 5.4 or higher
2. J2Store 3.2.x or higher
3. Joomla 3.x or higher

## Installation <a id="installation"></a>

1. Download Culqi payment plugin from our site’s extensions section and install it using Joomla installer.
2. After installing the plugin, go to J2Store &gt; Setup &gt; Payment methods and enable Payment Culqi.
3. Once enabled, open the plugin to configure the basic settings. \

   **Configuration**

**Payment option title** Enter the title for the payment option. The text entered here will be displayed at payment method step during checkout.

**Plugin Display Image** The image added here will be displayed while payment options are listed in the checkout page.

**Card details display format** Choose whether the card detail form should be displayed in a pop form or in normal checkout form.

**Commercial Code** Enter your commercial code associated with your culqi account.

**Secret API key** Enter secret API key associated with your culqi account.

You can get commercial code and secret API keys by logging into your culqi account. After you logging in, go to Development tab and click on API Keys.

Copy your Commercial Code and paste it in plugin’s settings. To know your secret API key, click on See under the column Key. Popup will show your secret API key. Copy and paste it in plugin’s settings.

![credentials](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/culqi-payment/culqi-api-credentials.png)

**Culqi User ID / User Email** Enter the User ID or Email ID associated with your culqi account.

**Use Sandbox Mode** Culqi offers a testing suite called Sandbox. Before going live, you can test your store using the culqi’s sandbox feature. Set this option to YES enable sandbox mode.

**Sandbox Commercial Code** If you are using culqi in sandbox mode, enter the commercial code associated with your culqi’s sandbox account.

**Sandbox secret API key** Enter secret API key associated with your culqi’s sandbox account.

**Sandbox Culqi User ID / User Email** Enter User ID or Email ID associated with your culqi’s sandbox account.

**Article ID for Custom Thanks Message** You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

**Geozone** By selecting geo zone here, you can restrict this payment method to only customers of that geo-region. Choose ALL to show this payment method to all customers.

**Display text on selection** Enter the text to be displayed when customer selects this payment method during checkout. You can also enter a language constant as a value here if you are using multi-lingual site and then write a language override.

**Display text before payment** Enter the text to be displayed at order summary screen before customer makes the payment.

**Display text on after in payment** Text entered here will be displayed when customer completes the payment.

**Display text on error in payment** Text added here will be displayed when an error occurs during payment process.

**Payment button text** Value entered here will be added as the name of the payment button. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.

**Debug** Choose YES to enable the debug mode. If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory. DO NOT select YES in the live site.

![culqi](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/culqi-payment/culqi-plugin-config.png)

**Frontend**

![popup](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/culqi-payment/culqi-popupform.png)

![checkout](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/culqi-payment/culqi-demo-checkout-form.png)

