# Post Finance

The plugin integrates Post Finance payment with J2Store Joomla eCommerce solution.

PostFinance’s payment solutions offer you secure and fast payment collection. As an online shop operator, you can process all standard payment methods.

### Requirements <a id="requirements"></a>

1. PHP 5.4 or greater
2. Joomla 3.x
3. J2Store 3.2.x or greater

## Installation <a id="installation"></a>

* Use the Joomla installer to install the plugin.
* In the backend, go to J2store Dashboard -&gt; Payment methods and enable plugin.
* Open the plugin and enter the parameters \(read the explanation about each parameter given below\)
* Save and close it.

## Required Post finance settings <a id="required-post-finance-settings"></a>

**Default operation code**

* Sale: This will enable you to receive instant payment.
* Authorisation: This you have to either manually or automatically capture it.

For Sale, a successful payment will return Status code 9 and for Successful Authorisation, the status code is 5. Both the cases will be treated as Success and Confirmed by thePost finance plugin.

NOTE: If you are selling digital goods, it is advised to use SALE as operation

The following parameters in your Post finance account \(Technical Information\) should be set as instructed below.

Hashing method \(Tab: Global security parameters\)

Should be set to SHA-1. The plugin will not work with the other methods. Refer the image below.

![hashing method](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/post-finance/hashing_method_ogone.png)

**Checks for E-Commerce \(Tab: Data and origin verification\)**

URL of the merchant page containing the payment form that will call the page: orderstandard.asp: Leave the data origin url empty

![check post finance](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/post-finance/ecommerce_check_postfinance.png)

**Post sale configuration : \(Tab: Transaction feedback\)**

This is required to update our database after the payment is done. Under the heading “Direct HTTP server to server request”, set both the URLs of the merchant’s post payment page as below:

http://www.yourdomain.com/index.php?option=com\_j2store&view=checkout&task=confirmPayment&orderpayment\_type=payment\_postfinance&paction=process&tmpl=component” target = “\_blank”rel = “noopener”&gt; click here

Request method: POST

\(see the picture below with example urls.\)

![feedback](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/post-finance/transaction_feedback_ogone.png)

## Plugin Configuration <a id="plugin-configuration"></a>

**Payment option title** The value entered here will be used as the title for the payment. Customer will see this value when he checks out.

**Plugin display image** This image will be displayed while payment options are listed in the checkout page.

**PSPID** This is your Unique Merchant ID provided by the Post finance. Enter the PSPID associated with your Post Finance’s Account.

**SHA-IN key** This is the SHA-1 IN signature set up by you in the Post finance settings \(see below for the required settings to be done at your Post finance account\). This ensure security of your transaction.

**SHA-OUT key** This is the SHA-1 OUT signature set up by you in the Post finance settings \(see below for the required settings to be done at your Post finance account\)

**Hash Method** Select Hash method \(SHA-1, SHA-256, SHA-512\) associated with your postfinance account. It should be set to SHA 1.

**Language** Payment form page will be displayed in the language chosen here.

**Use sandbox** Post finance offers a testing suite. Before going live, it is advised to test your store using the Post finance test server. Read more about Post finance test account at the Post finance’s official website

NOTE: IN LIVE SITE, THIS SHOULD BE SET TO NO.

j2store_postfinance_tp

Create new template and its path to here so that your payment form page will be displayed in the template style chosen here.

**Article ID for Thank You message** You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

**Display text on selection** The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-&gt; Language Manager-&gt;Overrides and create overrides for the language constant in all your languages.

**Display text before payment** The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on after payment** The text entered here will be displayed when customer completes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment** The text entered here will be displayed to the customer when there is an error in the payment process. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text if customers cancels payment** The text entered here will be displayed to the customer when he cancels the payment at the gateway \(NOT in your site\). You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment button text** Text entered here will be added as the name of the payment button. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.

**Debug** Choose YES to enable the debug mode. If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory. DO NOT select YES in the live site.

**Support** Still have questions? You can post in our support forum: [click here](http://j2store.org/forum/index.html)

Thank you for using our extension.

