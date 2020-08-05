# Authorize.Net plugin

This Plugin enables you to receive payments via Authorize.Net Payment Gateway. Visit [click here](http://authorize.net/) to know more about the payment gateway.

## Requirements <a id="requirements"></a>

* PHP 5.2 or higher
* Joomla 2.5.x
* J2Store 1.0 or above

## Installation Instructions <a id="installation-instructions"></a>

1. Use the Joomla installer to install the plugin.
2. In the backend, go to Extensions-&gt;Plugin Manager and open the Heartland Payment plugin. \(type = j2store\).
3. Enable the plugin.
4. Enter the parameters \(read the explanation about each parameter given below\).
5. Save and close it.

Now you can see the Authorize.net Payments as an option during the Checkout process.

## Parameters <a id="parameters"></a>

**Authorize.net Login ID**

This is your Merchant Login Id given by the Authorize.net

**Authorize.net Transaction Key**

Transaction key provided by the authorize.net

**Authorize.net MD5 Hash**

This is an additional security feature of Authorize.net. But use with care. If you dont know what you are doing, pleaseleave this blank. This is optional parameter.

**Use SSL to post back to Authorize.net?**

If you are using SSL certificate \(https\), enable this. If you dont know what SSL is, better leave it as No.

**Use Authorize.net Sandbox**

Authorize.net offers a testing suite called Sandbox. Before going live, it is advised to test your store using the sandbox feature. Read more about Sandbox at Authorize.net.

NOTE: To receive payments \(except during testing\), you DONT have to enable this.

\*\*IN LIVE SITE, THIS SHOULD BE SET TO NO. \*\*

**Sandbox Login ID**

Your sandbox login ID provided by Authorize.net.

**Sandbox Transaction Key**

You transaction key provided by the sandbox.

**Sandbox MD5 Hash**

Md5 has provided in sandbox.

**Thanks Msg Joomla Article ID**

You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

Still have questions? You can post in our support forum: [click here](http://j2store.org/forum/index.html)

Thank you for using our extension.

\[HOW TO\]Solve “Error processing payment Invalid Order This transaction cannot be accepted.” It seems to be using of expired transaction key.

**To regenerate the transaction key :**

1. Log into your Merchant Interface at [click here](https://account.authorize.net/)
2. Click Account from the main toolbar.
3. Click Settings in the main left-side menu.
4. Click API Credentials & Keys.
5. Enter your Secret Answer \(the answer to your Secret Question configured at account setup\).
6. Select New Transaction Key.
7. To disable the old Transaction Key, click the check box labeled Disable Old Transaction Key Immediately.

