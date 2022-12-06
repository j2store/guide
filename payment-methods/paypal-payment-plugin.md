# Paypal payment plugin

The plugin integrates PayPal Website Payment Standard method with your J2Store shopping cart. You need either a PayPal account in order to take payments

Are you looking to troubleshoot your PayPal integration? We have answered most of the common problems. So read carefully

## Introduction <a href="#introduction" id="introduction"></a>

Paypal standard plugin for J2Store allows you to accept payments via Paypal Payment Gateway. This uses the Paypal’s Website Standard Payment. Customer will be redirected to Paypal to make payment securely

## Requirements <a href="#requirements" id="requirements"></a>

&#x20;PHP 5.2 or higher Joomla 2.5.x J2Store 2.0 or above

## Installation Instructions <a href="#installation-instructions" id="installation-instructions"></a>

1. Use the Joomla installer to install the plugin.
2. In the backend, go to Extensions->Plugin Manager and open the Paypal Paymentsplugin. (type=j2store).
3. Enable the plugin
4. Enter the parameters (read the explanation about each parameter given below)
5. Save and close it.

Now you can see the Paypal Payments as an option during the Check out process.

## Parameters <a href="#parameters" id="parameters"></a>

**Payment option title:** Enter the title of the payment plugin which you wish to display in the checkout page.

**Plugin Display Image:** Choose the image which you wish to display when the payment options are listed.

**Paypal Email Address** This is your original paypal email/merchant email address, which you have used in Paypal.

**API Username** Enter the API username associated with your PayPal live account.

**API Password** Enter the API password associated with your PayPal live account.

**API Signature** Enter the API signature associated with your PayPal live account.

Not sure where to find your API signature? Read the documentation below: [Click here](https://www.jotform.com/help/284-how-to-obtain-paypal-api-credentials/)&#x20;



NOTE: The API username, password and the signature are optional fields. These fields are required only when you use the subscription app or when you have an issue with receiving the IPN callbacks from Paypal. If you are using a personal account, then you can just fill in your PayPal Merchant Email (of your personal account) and start using the plugin. It is not necessary to fill-in the API Keys.

\*\*Check Paypal credentials: \*\*

Click on this to check whether the enter credentials are accurate.

Choose the callback url to be used for IPN notifications

The URL selected here will be set as dynamic IPN url instead of the URL which you have configured in your PayPal account.

* Default url : The default url is the normal query string url used for IPN Notifications. This will work for 99% of the users. If it does not work in some cases, you could try any one of the following alternative urls.http(s)://www.example.com/index.php?option=com\__j2store\&view=checkout\&task=confirmPayment\&orderpayment_type=payment\_paypal\&paction=process
* Alternative - 1 : It is the alternative callback url that uses the callback view.http(s)://www.example.com/index.php?option=com\__j2store\&view=callback\&method=payment_paypal\&paction=process
* Alternative - 2 : It is the Proxy of default url. Sometimes, the PayPal IPN server truncates the query strings. It happens very rarely and you can check the IPN history in your PayPal account to see if PayPal is truncating. Login to your PayPal account and then go to: to view the IPN history. If it does truncates the query strings, you can use this url http(s)://www.example.com/plugins/j2store/payment_paypal/payment_paypal/tmpl/notify.php

If you are using any firewall like Admin Tools PRO, you might have to add exception to IPN url you have selected to use. PayPal does a server-to-server remote post. Most firewalls will block remote post requests.

**Validate IPN:** Customers can receive instant payment notification whenever a payment is made.

**Check Server TLS :**

Will check whether the available tLs version matches with the current paypal version.

**Use Paypal Sandbox**

Paypal offers a testing suite called Sandbox. Before going live, you can test your store using the Paypal’s sandbox feature. Read more about Paypal Sandbox at developer.paypal.com.

**Paypal Sandbox Merchant Email**

Your paypal sandbox email.

**Sandbox API Username**

Enter API username associated with your PayPal sandbox account.

**Sandbox API Password**

Enter API password associated with your PayPal sandbox account.

**Sandbox API Signature**

Enter API signature associated with your PayPal sandbox account.

**Check paypal Credentials**

Check whether the entered credentials are accurate.

**Show billing agreement :**

Choose whether the customer billing agreement text is to be displayed for subscription products.

**Billing agreement text:**

Enter the billing agreement text which you wish to display in the payment page.

**Surcharge Percentage**

You can collect a percent of the total order value as surcharge / fee for using the Paypal option from your customers using this option. You can enter a value here (for example: 2 ). If you enter 2 here, then 2 % of the total order value will be added as a handling cost to the order.

This is optional parameter.

NOTE: DO NOT enter any symbol like % here.

Leave empty if you dont want to charge.

**Surcharge Fixed Value :**

You can collect a fixed surcharge / fee for using the Paypal option from your customers in addition to the order value. You can enter a value here (for example: 2 ). If you enter 2 here, then 2 will be added as a handling cost to the order.

Leave empty if you dont want to charge.

This is an optional parameter.

**Article ID for Thanks you message**

You can create an article to say thanks, provide some information or instructions to the customers, who purchased in your online store. Enter the Article ID here. This will show,when customers return from the paypal.

**Geozone**

By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.

**PayPal Callback Text**

By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.

**Logo Image for display in Paypal**

The URL of the 150x50-pixel image displayed as your logo in the upper left corner of PayPal’s pages. Default: your business name (if you have a Business account) or your email address (if you have Premier account). If this is not working, try using the Custom Header Image param above. This is an optional setting.

**Custom Header Image**

The URL to your logo so. This image will be displayed on the top of PayPal’s checkout page instead of your merchant name.

WARNING! It must be an HTTPS URL, otherwise your clients willreceive warnings about insecure content. This is an optional parameter.

**Header Background Colour**

The hex-code of your PayPal checkout page’s header, e.g. FFFFFF for white (note: place no # in front the hex value) This is an optional setting.

**Header Border Color**

The hex-code of your PayPal checkout page’s header border, e.g. FFFFFF for white (note: place no # in front the hex value) This is an optional setting.

**Display text on selection**

The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below

Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON\_SELECTION.

Now you can go to Joomla admin-> Language Manager->Overrides and create overrides for the language constant in all your languages.

**Display text before payment**

The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order**

The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment**

The text entered here will be displayed to the customer when there is an error in the payment process.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on cancel payment**

The text entered here will be displayed to the customer when he cancels the payment at the gateway (NOT in your site).

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment Button Text**

The text of the payment button. The button will be displayed at the final checkout step.

**Debug:**

Enable this to log the responses and request of the payment plugin. Do not set this in live site.

## SCA compliance: <a href="#sca-compliance" id="sca-compliance"></a>

To know more information on the SCA compliance for the Paypal plugin, click [click here](http://docs.j2store.org/frequently-asked-questions/sca-support-for-payment-plugins)

## Troubleshoot PayPal Related Issues <a href="#sca-compliance" id="sca-compliance"></a>

To troubleshoot PayPal related issues, click [click here](https://docs.j2store.org/troubleshooting-guide/troubleshooting-paypal-related-issues)
