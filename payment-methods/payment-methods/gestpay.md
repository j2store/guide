# GestPay

## Introduction <a id="introduction"></a>

The plugin integrates GestPay payment gateway with K2Store.

## Installation <a id="installation"></a>

You can install the plugin through the standard Joomla installer.

## Configuring your GestPay Backoffice <a id="configuring-your-gestpay-backoffice"></a>

There are two aspects you have to configure at your GestPay Backoffice

**Authentication configuration** You will have to authendicate the IP address of your site.

* Login to your GestPay Backoffice.
* Go to Configuration → IP addresses.
* Add the IP address \(es\) of your site there.

GestPay identifies the merchant requesting the encryption service through the WSCryptDecrypt web service by comparing the calling server IP address to theIP addresses configured in the profile associated with the Shop Login used for the call. If the calling server is not recognised, the transaction process ends anda specific error is returned. In the Configuration – IP Addresses section of the Back Office environment, themerchant can enter up to a maximum of 10 IP addresses \(if calls to GestPay originate from a server.

**Response URL**

Login to your GestPay Backoffice. Go to Configuration → Responses section Enter the following url in URL for positive response and URL for negative response fields. If your site DOES NOT have SSL , then use the following url

```text
http:///index.php?option=com_j2store&view=checkout&task=confirmpayment&orderpayment_type=payment_gestpay&paction=process
```

if you have SSL installed, then use the following u

```text
https:///index.php?option=com_j2store&view=checkout&task=confirmpayment&orderpayment_type=payment_gestpay&paction=process
```

## Configuration of the Plugin <a id="configuration-of-the-plugin"></a>

**Payment Option title:** Enter a name that will be shown in the payment methods selection during the checkout process. Default Gestpay

**Shop Login :** Enter the shop login provided by GestPay

**SSL Mode:** Do you want to use SSL \(https\) to communicate with the GestPay server ? Ifyes, set this to YES.

\*\*IMPORTANT: \*\* You should have installed SSL Certificate and applied it through the site. You should contact your hosting service provider to install SSL certificatein the site.

Only set this to YES, if you have SSL installed and enabled. Otherwise set this to NO.

**Use GESTPAY Test Server :** If you would like to test the plugin using the TEST server of GestPay, set this to yes.

Transactions will go to the test server and no real payments will be made.

\*\*IMPORTANT: \*\* NEVER set this to YES in a live site.

Article ID for custom thank you message: You can create an article with a message and enter its ID here. The message will be shown to the customer after completion of the purchase.

**Debug :** Enable this to debug the plugin. Never set this to YES in a live site.

