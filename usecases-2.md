# Usecases

## Receiving payments in 3 installments: <a id="receiving-payments-in-3-installments"></a>

Lets suppose you have a product whose cost is quite high.You might feel that you could attract many customers when the product is sold in installments.

Now that we re all set to receive payments in fragments, you might also want an effective way to maintain the orders and their payment schedules.

This can be done efficiently choosing the partial payment mode as PLANS.

## Plans <a id="plans"></a>

Lets suppose that you have a couch whose price is around 2000 $ and you are planning to get the payment in 4 pieces. In that case you could create a plan with the partial payment app called 4 installments as shown in the below screenshot:

![ppusecase1](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase1.png) For the above set up the users will be allowed to pay for the couch like this:

![ppusecase front](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase1front.png) So now that the user places the order and completes the first installment,you might wonder how the rest of the payment would be kept track of.

Here comes the order schedule that will keep you free of your worries about payments.Navigate as per the screenshots given here:

![ppusecase order1](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase1order1.png)

![ppusecase order2](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase1order2.png)

![ppusecase order3](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase1order3.png)

In this case when the due date approaches, the users and the store administrators would be notified.

## Receiving percentage of total amount as deposit: <a id="receiving-percentage-of-total-amount-as-deposit"></a>

Lets take the same instance of selling a couch to illustrate this feature as well: But this time we are going to get a percentage of the total amount as deposit and the remaining later. For this we might make use of the percentage type under partial payment type.

## Percentage <a id="percentage"></a>

This type is a simpler version of the plan type.It has all the features alike plan mode except for setting up the installment duration. Now we are planning to collect 25 % of the total amount as initial deposit.

![ppusecase 2](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase2.png)

![ppusecase2 front](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase2front.png) The remaining payment will be scheduledlike this:

![ppusecase2 order](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase2order.png)

## Collecting a fixed amount as the initial deposit: <a id="collecting-a-fixed-amount-as-the-initial-deposit"></a>

In the case of selling a couch you wish you could get $500 out of $2000 as the initial payment.

This could be achieved by choosing the partial payment type as Fixed price and specifying the amount like this one:

![ppusecase3](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase3.png) The product page will be like this:

![ppusecase3 front](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase3front.png) Orders willbe scheduled for the future payment like this:

![ppusecase3 order](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase3order.png)

## Exempt a product from the global settings: <a id="exempt-a-product-from-the-global-settings"></a>

If you wish to configure partial payment in another way when compared to the normal global settings then that is always possible with the product level settings.

When a product-level setting is configured for partial payment that would override the global setting.

If your site sells furniture and you wish to establish a different setup for Cabinets alone while the others go with the global setting, then this is how it could be achieved:

* Open the product article for which you would like to sset up different partial payment settings.
* Click on the ‘Apps’ option on the left side menu.
* For example if you wish to set up fixed payment as the mode for this product alone regardless of the global settings, then this is how it would be done:
* ![ppusecase4 product](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase4product.png)

This being the setting, the product cabinet will have a different setting when compared with the others:

## Global Settings: <a id="global-settings"></a>

![ppusecase4 global](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase4global.png)

## Product-level settings: <a id="product-level-settings"></a>

For the Product-level settings mentioned earlier this is how the product Cabinet will behave in the front end irrespective of the global app settings:

![ppusecase4 product front](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/usecases/app_partialpaymentusecase4productfront.png)

