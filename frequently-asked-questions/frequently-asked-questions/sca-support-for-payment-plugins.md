# SCA support for payment plugins

## SCA support for payment plugins <a id="sca-support-for-payment-plugins"></a>

In the European union, a new regulation for online payments would be rolled out in September 2019. This would require your payment plugins to be compliant to the SCA regulation.

## What is SCA: <a id="what-is-sca"></a>

Strong Customer Authentication \(SCA\) is a new European regulatory requirement to reduce fraud and make online payments more secure. To accept payments once SCA goes into effect, you will need to build additional authentication into your checkout flow.

Strong Customer Authentication \(SCA\) \([https://stripe.com/docs/strong-customer-authentication](https://stripe.com/docs/strong-customer-authentication)\), a new rule coming into effect on September 14, 2019, as part of PSD2 regulation in Europe, will require changes to how your European customers authenticate online payments. Card payments will require a different user experience, namely 3D Secure, in order to meet SCA requirements. Transactions that don’t follow the new authentication guidelines may be declined by your customers’ banks.

## Will I need to update my payment plugins? <a id="will-i-need-to-update-my-payment-plugins"></a>

Yes, we are in the process of updating our payment plugins to ensure that they support the SCA compliance.

This update would be rolled out before September, when the regulations come into effect.

**Are Paypal and Stripe compatible with SCA:**

    **1\) Paypal Standard:**

    With the standard version of Paypal, the transactions happen at the payment gateway and not on the Merchant site.

    So, Paypal would handle the compliance by itself.

    Store owners need not worry about the compliance since the transaction occurs outside of the store.

    **2\) Paypal PRO:**

    The latest version of Paypal PRO\(2.15\) does support SCA regulations.

    **3\) Stripe:**

    ****As far as Stripe is concerned, the latest version of Stripe the **In-built mode** supports SCA regulations.

    You will have to update Stripe to the latest version\(1.53\) and set the option **Enable payment intent in in-built form to YES in the plugin settings.**

**SCA supported cards for testing:** 

You might want to use only these cards for testing Stripe SCA compliance:

[https://stripe.com/docs/payments/cards/saving-cards](https://stripe.com/docs/payments/cards/saving-cards)

**Stripe Hosted checkout:**

With the purchase of Stripe integration, there comes another additional plugin called Stripe checkout\(Hosted\).

You could find this plugin at the My Downloads page of the J2Store site.

**PS: With this plugin, you need not worry about SCA compliance since the transactions occur in Stripe gateway.**

More info about this can be found here:

[https://docs.j2store.org/payment-methods/stripe/](https://docs.j2store.org/payment-methods/stripe/)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/13074122822/original/5h_L1OTa3oFalZ2UR7nbuJv9tAL6LrTiUQ.png?1565934569)

**Stripe for subscription products:**

We have rolled out an update\(version 1.53\) starting from which, Stripe would support SCA regulations on recurring payments, which is for subscription products.

Following are the SCA supported cards for testing:

[https://stripe.com/docs/payments/cards/saving-cards](https://stripe.com/docs/payments/cards/saving-cards)

**NOTE: SCA authentication popup would come up only if you use the above SCA supported cards to test.**

**4\) Other payment gateways:**

    If the payment occurs in the payment gateway, then SCA compliance would be handled by the payment gateway itself.

    If the transactions occur in the merchant site, then please drop us a support request to check the compatibility.

