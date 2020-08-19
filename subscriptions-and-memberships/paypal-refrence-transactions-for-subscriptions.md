# Paypal Reference Transactions for Subscriptions

This system makes it possible to sell multiple subscriptions, change recurring totals and billing schedule, and allow customers to switch subscriptions.

However, there is a catch: PayPal must enable Reference Transaction support on your PayPal account in order to use this.

How do I get Reference Transactions Enabled with PayPal?

To request that PayPal turn on Reference Transactions, call your local PayPal Support Help Center. Find the [phone number at Contact](https://www.paypal.com/selfhelp/contact/call)

Tell PayPal that you are specifically calling so a PayPal Specialist can enable Reference Transactions on your account. They may try to help you set up recurring payments with a button — that is not what you want. They need to transfer you to a specialist who will ask you for your PayPal account information \(email address\), and then tell you that they filed a ticket, and you will hear back from PayPal via email on whether Reference Transactions have been enabled or not.

## Email Application <a id="email-application"></a>

You can also contact PayPal via email.

1.  [Log into your PayPal account](https://www.paypal.com/signin/)
2.  Go to the [Email Contact Form](https://www.paypal.com/selfhelp/contact/email/t_s)
3. Choose topic: My Account.
4. Choose sub-topic: Changing/Updating Account Information.
5. Copy and paste the message below, inserting your PayPal email address and name.
6. Wait for a reply.

![paypal support](https://raw.githubusercontent.com/j2store/doc-images/master/subscriptions-and-memberships/paypal-reference-transactions-for-subscriptions/paypal-support-screenshot.png)

## Example Message to send to PayPal <a id="example-message-to-send-to-paypalhello"></a>

```text
Hello,
I need this feature to sell recurring subscription products via J2Store.

Kind regards,

Your Name
Gotcha: Respond to the Autoresponder```


In an effort to reduce support, PayPal may send you a response from an auto-response message with some links to documentation.

### Hidden in this auto-response is the following:

If we haven’t answered your question, please reply to this email and our team will answer you as soon as possible.

> You also need to respond to the auto-response before your support ticket is submitted to PayPal.

### Will My Account Qualify for Reference Transactions?

PayPal does have a set a requirements that need to be met before they enable support for Reference Transactions on your account.

Unfortunately, PayPal does not publish these requirements and based on anecdotes from customers, the requirements can be different for different businesses.

Some things that store owners have mentioned PayPal require are:

1. High personal credit (FICO) score for US based PayPal Business accounts
2. Business plan
3. Average transaction price
4. Number of repeat customers
5. Number of Reference Transactions per customer
6. Revenue forecast and/or projected total revenue volume from Reference Transactions
7. Demonstrate a clear business rationale behind the request
8. Show the signup flow for customers in regards to Reference Transactions.
9. Proof that you will show clear terms and conditions for customers  in regards to Reference transactions and how to cancel once they sign up.
10. Written statement as to why you need Reference Transactions and how you will use it for your business.

In terms of revenue forecasts, we have had reports that UK based PayPal accounts may require minimum forecast of £6,000 month or more revenue.
```

## Limitations of PayPal Standard with Subscriptions

### Required Subscribers to Have a PayPal Account:

PayPal requires **subscribers to have a PayPal account** for automatic recurring payments. This means that customers will **not** be able to check out without having a PayPal account or by creating one during the checkout process.

### Currency Limitations:

Please make sure that the merchant's currency is one that is supported by PayPal. If your store's currency is not supported by PayPal, then IPN notifications wouldn't reach the store and as a result, order statuses of concerned subscriptions would not be updated automatically.

### PayPal Merchant Accounts:

PayPal Standard also limits the PayPal account holder from using the same PayPal account on multiple websites. As a result, **PayPal Standard can only be used to sell subscriptions on one website**.

