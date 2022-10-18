# Bulk discounts

Encourage customers to purchase more by providing bulk discounts depending on the ordered quantity and on the specific product.

Bulk discounts can be defined at site-wide (globally), category wise or per product wise. Provide a fixed per product discount or percentage of the total purchase. The plugin implements a greater flexibility in providing discounts without requiring the customers to apply a coupon.

You can also restrict the application of the discount depending on the customer groups.

**Requirements**

* PHP 5.4 or higher
* Joomla 3.3 or above
* J2Store 3.2.x or above

**Installation Instructions**

1. Use the Joomla installer to install the app.
2. Go to J2store -> Apps and enable app.
3. Open the App Bulk Discount.

&#x20;

![Enabling bulk discounts](https://raw.githubusercontent.com/j2store/doc-images/master/apps/bulk-discounts/bulkdiscount\_enable.png)

\*\*Priority of the discounts:

\*\*Here is how the priority of the discount rules is decided. Following is the priority from high to low.

* **Product-level settings**
* **Category-level settings**
* **Global settings**

That is, when there is a product-level discount set and a category-level discount set, the product-level rule would be of higher priority than the category-level rule.

The same goes for the global rule as well. At any cost, the product-level setting would be given the high priority.

Also, when there is a category-level discount set, the product level setting for enable bulk discount parameter should be NO. If not, the product-level setting would be given priority, thus overriding the category level setting.

## Parameters <a href="#parameters" id="parameters"></a>

**Basic Settings**

* **Display name**

Text entered here will be displayed as promotion display text.

* **Remove discount if a coupon is used by the customer (prevents customers getting double discounts)**

Set this to Yes to remove the discount when customer used the coupon.

* **Display promotion Message In Cart**

Set this YES display the promotion message in the cart if any bulk discount not applied.

* **Apply Bulk discount for**

**Cart Qty :** This will apply the discount globally i.e. based on the cart quantity. This will work only when you enable the bulk discount globally in Global discount settings.

**Line item Qty :** This will apply the discount based on the product. You can set discount to the product individually in the apps tab on j2store cart. Once you enabled Line item Quantity, the discount will be applied to the individual products.Refer the below image for setting discount for the product individually.

![Product-level discount](https://raw.githubusercontent.com/j2store/doc-images/master/apps/bulk-discounts/bulkdiscount\_product.png)

* **Product discount price display format**

\*\*Per quantity Discount: \*\*

The discount is based on the product.

\*\*Total Discount: \*\*

Discount is the based on the total purchase amount of a particular order irrespective of the quantity.

* **Display discounts in**

Display the discount information in any one of the three options(Products view only, Category view only, Both product and category view).

![Global settings for bulk discount](https://raw.githubusercontent.com/j2store/doc-images/master/apps/bulk-discounts/bulkdiscount-global-basic.png)&#x20;

**Global discount settings**

You can use these options when you are trying to offer a site-wide discount on your products.\


Also, when you are trying to set up same type of discounts for a majority of the products while a very few products require change, then you can define the discount here and override this setting at the product level or the category-level.\


* **Enable bulk discount globally**

Set this YES will enable the global discount function.

* **Discount type**

\*\*Fixed amount per product : \*\*

Enable this will calculate the discount on fixed price.

\*\*Cart Percentage : \*\*

Enable this will calculate the discount based on percentage.

\*\*NOTE: when you set up a cart percentage discount, the discount information would be displayed only on the cart page. A table showing the discount would not be available for the fixed price discounts.

* **Promotional text to show under each item in the cart(only for cart page)**

Custom text entered here will be displayed under each product in the cart.

* **Single Quantity Class**

Here you can set the custom class, if you set the quantity for one and above.

![Global settings for bulk discount](https://raw.githubusercontent.com/j2store/doc-images/master/apps/bulk-discounts/bulkdiscount\_global-global.png)

**Setting up bulk discounts for particular categories:**

This app will allow you to set discount by category wise. Go to Content > Categories > Open the category(to which you want to set bulk discount) > Bulk Discount tab.

* **Enable Bulk Discount**

Set this YES to enable the bulk discount for the category.

* **Apply Bulk discount for**

**Cart Qty :** This will apply the discount globally i.e. based on the cart quantity. This will work only when you enable the bulk discount globally in Global discount settings.

**Line item Qty :** This will apply the discount based on the product. You can set discount to the product individually in the apps tab on j2store cart. Once you enabled Line item Quantity, the discount will be applied to the individual products.

* **Discount type**

\*\*Fixed amount per product : \*\*

Enable this will calculate the discount on fixed price.

\*\*Cart Percentage : \*\*

Enable this will calculate the discount based on percentage.

* **Promotional text to show under each item in the cart(only for cart page)**

Custom text entered here will be displayed under each product in the cart.

![Category-discounts](https://raw.githubusercontent.com/j2store/doc-images/master/apps/bulk-discounts/bulk\_discount\_category.png)

\*\*Product level bulk discounts:

Bulk discount plugin offers a product-level setting. So, if you are trying to set up product-specific discounts, then that is also possible by following the below steps:

* Navigate to J2Store->Catalog->Products->choose the product for which you are trying to offer discounts.
* Click on the J2Store cart tab and select the apps tab on the left pane.
* Set the enable bulk discounts option to YES.
* **Discount type**
* **Fixed-amount per product -** To set up a fixed price discount for the product choose this option. For example: 20$ discount, or a 50$ discount.
* \*\*Cart percentage - \*\*To set up a percentage discount at the cart page for a particular product, choose this option. For example: a 20% discount, a 30% discount. As the name goes, this discount would be applied only at the cart level.&#x20;
* \*\*Promotional text to show under each item in the cart(only for cart page) \*\*

This setting lets you mention a promo message at the cart page alone. The text entered here would be displayed at the cart page.

* \*\*Combine product quantity in cart \*\*

When this option is checked, the quantities of the product would be calculated cumulatively and discount would be added accordingly. For example: If you are setting up a discount for a T-shirt product, and the t-shirt has options, say, size as Small, Medium and Large. If the user chooses to buy a shirt of the size small and one shirt of the size medium, then should these two quantities be added?

* Next comes the part where you choose the quantity range, usergroup and the discount value.

\*\*Product-level fixed price discount: \*\*

![Product level fixed price](https://raw.githubusercontent.com/j2store/doc-images/master/apps/bulk-discounts/bulkdiscount-pro-level-fixed-price.png)

\*\* Frontend view:\*\*&#x20;

![Frontend view of discount](https://raw.githubusercontent.com/j2store/doc-images/master/apps/bulk-discounts/pro-level-fixed-frontend.png)

**Video tutorial**

&#x20;[![Bulk discounts](https://img.youtube.com/vi/51J1UkeRu3Y/0.jpg)](https://youtu.be/EGW0Ol5o3jA)
