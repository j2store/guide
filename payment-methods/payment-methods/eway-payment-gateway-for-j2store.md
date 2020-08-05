# eway Payment Gateway for j2store

## Introduction <a id="introduction"></a>

The eWAY plugin for J2Store allows you to take credit card payments directly on your store without redirecting your customers to a third party site to make payment.eWay is one of the popular payment gateways in Australia, New Zealand and United Kingdom processing credit card transactions.eWay helps you accept credit card payments securely in your store front.

There are two plugins available based on two methods

1. eWay Rapid \(based on the New Rapid 3.1 API\) - Recommended
2. eWay Direct \(old API \) - Not recommended.

## Installation <a id="installation"></a>

Download the plugin file and install it via the Joomla Extension Manager.

**Upgrading from old Direct method to new eWay Rapid**

1. Login to your MYeWay merchant account and get the API Key. Or you can contact eWay to get your API Key and API Password from them.
2. Download the eWay Rapid plugin from our My Downloads section and install it.
3. Open the plugin to enter the API Key and configure other fields.
4. Disable the old eWay Direct plugin.

## Configuration - eWay Rapid <a id="configuration---eway-rapid"></a>

Go to J2Store - Payment Methods and open the eWay Rapid plugin

**eWay Customer API Key:** Your eWay Customer API Key \(obtained from the MYeWAY merchant console\)eWay Customer Password: Your eWay Customer Password

**Payment Type** Choose whether you want to load the payment methods in an iframe or redirect the customer to eWay using the transparent redirect

**Payment ModeAuthorisation:** If you choose this mode, then payment from customer will be authorized and kept in hold. It will not be captured and credited to your account. You will have to manually capture the payment from eWay Merchant consoleSale Default mode. eWay will capture the payment and credit it to your account immediately.

Use eWay Sandbox Turn this on to use the Test system provided by eWay. IMPORTANT NEVER EVER set this to YES, when your site is LIVE.

**Article Id for Thank you Message** You can create an article with a custom message \(example, thanking the customer for the order\) and enter its ID here. This will show up after the customer completes the purchase.

Configuration - eWay Direct Old method. Not recommended by eWay. Consider using the eWay Rapid

IMPORTANT: eWay Direct can only handle the Australian Dollor. So you should first set your default Currency is AUD.

**Customer ID:** Enter the customer ID provided by the eWay.

**Pay Method:** eWay offers three types of pay methods.

1. Real Time: Payment will be made realtime without CVV/CVN verification
2. Real time with CVN: Recommended method. This will verify the CVV/CVN value of the card
3. GeoIP and Anti-Fraud:This will send the customer IP address in order to verify the IP and check fraud based on Geolocation.

**Use eWay Sandbox:** Set this to yes to test your transaction using the Sandbox of eWay. Note: You should use the customer ID given in the sandbox instead of the live one.

**Article for Thanks Msg:** You can create an article with a custom message and enter its ID here. Customers will see this message after the payment.

