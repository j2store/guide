# Additional fee

## Requirements <a href="#requirements" id="requirements"></a>

1. PHP 5.4 or higher
2. Joomla 3.3 or above
3. J2Store 3.2.x or above

## Installation <a href="#installation" id="installation"></a>

1. Use the Joomla installer to install the app.
2. In the backend, go to J2Store Dashboard -> Apps as shown in the image below.
3. Click Enable in the Additional Fee app.

![Additional fee enable](https://raw.githubusercontent.com/j2store/doc-images/master/apps/additional-fee/addfee\_enable.png)

4\. Once the app is enabled, open the app to configure the settings and to setup the additional fee.

![Additional fee open](https://raw.githubusercontent.com/j2store/doc-images/master/apps/additional-fee/addfee\_open.png)

## Settings <a href="#settings" id="settings"></a>

Open the app and click the settings button on top to configure the app settings.

![Click settings](https://raw.githubusercontent.com/j2store/doc-images/master/apps/additional-fee/addfee\_clicksettings.png)

**Additional fee should be calculated per**

You can choose whether the additional fee should be applied based on cart or per product level.

* Order: This will apply the additional fee globally i.e. based on the cart.
* Line item: This will apply the additional charge based on the product. You can set additional fee to the product individually in the apps tab on j2store cart. Once you enabled Line item, the amount / charge will be applied to the individual products.

**Order price range based on**

Here you can define whether the order total after applying additional fee should be calculated based on subtotal or based on subtotal including shipping price.

**Auto apply additional fee in checkout ?**

Set **YES** will apply the additional fee at the checkout automatically. Set **NO** will hide the additonal fee displaying in cart page and checkout and it will display the checkbox at the payment step allowing customers to choose the fees.

**Display a checkbox in the following checkout step**

You can change the position of checkbox by selecting either **Display before shipping method** or **Display after payment methods**.

**Tax Profile**

Select your tax profile to display the additional fee as taxable.

&#x20;

![Settings](https://raw.githubusercontent.com/j2store/doc-images/master/apps/additional-fee/add-fee-settings.png)

## Additional Fee Setup <a href="#additional-fee-setup" id="additional-fee-setup"></a>

Open the app and click **Add New** button to create new one.

![Adding new rule](https://raw.githubusercontent.com/j2store/doc-images/master/apps/additional-fee/addfee\_clickaddnew.png)

**Name of the fee:** Enter the name for additional fee. The value given here will be displayed during checkout.

**Geozone:** Restrict applying additional charge based region. If you wants to apply extra charge only for customers from United States, then create the geozone for US and assign it here.

**User IDs:** You could also apply the charge only to specific customer by adding user id of the customers here. You can add multiple user ids with comma(,) separated.

**User groups:** It is also possible to restrict additional fee by user group. The additional fee will be applicable to the customers belongs to the user group selected here.

**Amount:** Enter the amount to be charged.

**Fee value type:** Choose whether the additional charge should be the fixed price or based on percentage.

**Category list:** If you would like to apply the extra charge by category wise, then all you have to do is select the category to which the additional fee should be applied.

**Apply when category product quantity is greater than or equal to and Apply if category product quantity is less than or equal to:** If you wants to apply the fee for the particular quantity range of the product from the particular category chosen above, specify the quantity range here.

**Apply when total order quantity is greater than or equal to:** Enter the quantity range. For example, set quantity range **2**. So additional fee will be applied when the quantity reaches **2** or **above 2**.

**Apply if total order quantity is less than or equal to:** Additional fee will be applied when the quantity reaches the value entered here. For example, set quantity range **2**. So additional fee will be applied when the quantity reaches **2** or **less than 2**.

**Apply when total order value is greater than or equal to:** Additional fee will be applied when the total order price reaches the value entered here. For example, set value **50**. So the charge will be applied when order value becomes **50** or **above 50**.

**Apply if total order value is less than or equal to:** Additional fee will be applied when the total order price reaches the value entered here. For example, set value **40**. So the charge will be applied when order value becomes **40** or **less than 40**.

&#x20;

![Addnew](https://raw.githubusercontent.com/j2store/doc-images/master/apps/additional-fee/addfee\_new.png)

## Additional Fee Setup at product level <a href="#additional-fee-setup-at-product-level" id="additional-fee-setup-at-product-level"></a>

* Go to Article manager.
* Open the article / product > J2Store cart tab.
* Navigate to the Apps tab and click add new button to setup the additional fee for that product. Refer the below screenshot.

![Add new item](https://raw.githubusercontent.com/j2store/doc-images/master/apps/additional-fee/addfee\_lineitem.png)

### Frontend <a href="#frontend" id="frontend"></a>

If Auto apply additional fee in checkout is set to **NO**,

![Frontend view](https://raw.githubusercontent.com/j2store/doc-images/master/apps/additional-fee/addfee\_frontview.png)

If Auto apply additional fee in checkout is set to **YES**,

&#x20;

![Cart page with additional fee enabled](https://raw.githubusercontent.com/j2store/doc-images/master/apps/additional-fee/addfee\_front\_cart.png)
