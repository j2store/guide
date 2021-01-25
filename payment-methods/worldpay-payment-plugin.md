# Worldpay Payment Plugin

This plugin integrates J2Store with the WorldPay payment gateway.

**Installation** Go to Extensions Manager and Install the plugin by choosing the plugin pack.

**Configuration** World Pay configuration

Login to your Merchant Interface and go to Installation → Integration Setup

![worldpay](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/worldpay-payment-plugin/worldpay_payment_plugin.png)

![response](https://raw.githubusercontent.com/j2store/doc-images/master/payment-methods/worldpay-payment-plugin/payment_response_worldpay.png)



```text
https://yourdomainname.com/index.php?option=com_j2store&view=checkout&task=confirmPayment&orderpayment_type=payment_worldpay&paction=process&tmpl=component
```



{% hint style="danger" %}
Replace “yourdomainname.com” with your domain name.
{% endhint %}

**Payment Response Enabled** Check this check box. Only then the order status will be updated automatically, if payment is successful. Otherwise, you will see incomplete orders.

**Payment response password** DO NOT fill anything here. Leave it empty.

**MD5 Secret for transactions field** Enter a password / Key here. Remeber this as you have to enter this in the plugin setup as well.

**Signature Fields** Enter the following value to SignatureFields field in the Integration Setup in WorldPay: instId : cartId : amount : currency

**Plugin configuration** Go to Joomla admin-&gt;Plugin manager-&gt;WorldPay and open the plugin, fill in the params \(refer the explanations below\), save the plugin and enable it.

**Payment option title** Enter a name here. This will be displayed in the Payment selection page \(during checkout\).

**WorldPay Installation ID** Installation ID provided by the WorldPay. Login to your Merchant Interface and Go to Installations-&gt;test or production environment to see the Installation ID.

**Secret MD5 key** This is the key you have created in the previous step in your World Pay merchant interface.

> Use WorldPay Test EnvironmentIf you want to test your set up, set this to yes.

**Article ID for Thank you Message** Create an article in Article Manager with a thank you message to your customers and save it. And note down its ID. Enter this Article ID here.

The next five fields are used for shopper response displayed after the shopper pays.

**Response Heading** This heading will show as a title in the response page.

**Response message** A short message displayed under the response heading. This can be like an intro or a help text to your customer.

**Success message** This message will be displayed if payment is successful.

**Failure message** This message will be displayed if payment failed.

**Return Link Title** Title of the return link displayed in the shopper response.

**Support** Still have questions? You can post your questions in our support forum: [http://j2store.org/forum/index.html](http://j2store.org/forum/index.html)

