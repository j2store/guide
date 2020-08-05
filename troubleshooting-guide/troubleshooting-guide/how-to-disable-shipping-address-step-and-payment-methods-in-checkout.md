# How to disable shipping address and payment in checkout

Many owners of small online stores have asked us how to disable the Shipping address

and Shipping & Payment Method sections in the checkout. This guide explains the steps to hide the checkout steps.

## Hiding Shipping Address section <a id="hiding-shipping-address-section"></a>

**Step 1** Go to J2Store -&gt; Configuration -&gt; Cart tabSet the Enable Shipping address fields to No.

**Step 2** Open your products \(articles\) and make sure that the Enable shipping for this item is set to NO.

Now shipping fields will not show.

Hiding Shipping & Payment Method blocks

Go to Joomla admin -&gt; J2Store -&gt; Set up -&gt; Payment

Make sure that ONLY ONE payment plugin is enabled.

> IMPORTANT: If you are using the Paypal as payment method, just enable the Paypal Plugin. Make sure that other payment plugins are disabled.

Similarly, you should have ONLY ONE shipping method enabled. If you created and enabled two or more shipping methods, then you cannot disable this section.

Add the following CSS at the end of your template’s CSS file to hide the Shipping and Payment Methods blocks.

```text
#shippingcost-pane {
display: none;
}

#onCheckoutPayment_wrapper {
display: none;
}
```

Save.

Now the Shipping and Payment methods blocks won’t be displayed.

> NOTE: You cannot hide or skip shipping /payment methods step. You can just hide its contents. The customer will still have to go through this step and click the continue button in order to progress to the order summary page.

## Billing Address <a id="billing-address"></a>

You cannot disable the Billing address entirely. However, you can reduce the number of fields in the billing address section.

You can disable the fields via the Custom Fields manager.

**IMPORTANT: You should at least have the Email field enabled. The remaining could be disabled.di**

