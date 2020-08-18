# Limitations of PayPal Standard with Subscriptions

## Required Subscribers to Have a PayPal Account:

PayPal requires [subscribers to have a PayPal Account](https://docs.woocommerce.com/document/subscriptions/faq/#section-32) for automatic recurring payments, unless the account has registered for [Enhanced Recurring Payments](https://www.paypal.com/us/webapps/mpp/ua/us-erp-full#1) \(Paypal only offers Enhanced Recurring Payment to US companies\). This means that customers will not be able to check out without having a Paypal  account or by creating one during the checkout process.

## Currency Limitations:

If a payment is held at PayPal because it is in a currency not supported by the merchant’s PayPal account, when that payment is accepted at PayPal.com, PayPal does not send an IPN message to notify WooCommerce or Subscriptions that the payment has been completed. 

Because of the way that PayPal handles this, there is no way to automatically update the order’s status for the transaction. The store manager will need to manually update the order’s status in WooCommerce to reflect the successful charge.

## PayPal Merchant Accounts:

 PayPal Standard also limits the PayPal account holder from using the same PayPal account on multiple websites. PayPal does not allow you to set multiple IPN URLs in a single PayPal account. It also does not allow applications, which you could consider WooCommerce Subscriptions as one, to set different IPN URLs for each website. As a result, **PayPal Standard can only be used to sell subscriptions on one website**.

