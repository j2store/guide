# Easy checkout

With online shopping moving quickly, convenience is becoming a must for customers. Overcomplicating your check out process can result in lost sales and unsatisfied customers.One would think that fewer steps would make it easier for the customer to check out, but that is not always the case.

Here we are coming up with **Easy checkout** for J2Store that makes the checkout process quiet easier.

Easy checkout is nothing but an one-page checkout that displays all elements of a standard checkout including basket contents, billing and shipping address, shipping options, and payment information on one page. Originally, one-page checkouts were put into practice in an effort to simplify the check out process with fewer clicks and fewer pages.

It will be easier to complete as less steps can appeal to time-conscious customers.

**Requirements**

1. Joomla version 3.4 +
2. PHP version 5.6 +
3. J2Store 3.3.0

**Installation**

1. Download and install our Easy checkout component using Joomla installer.
2. After installing, go to Extensions &gt; Plugins and make sure that the plugin System - EasyCheckout has been enabled.
3. Once you enabled the system plugin, the J2Store’s normal checkout will be replaced and the single step checkout will be activated.

Few points that has to be remembered

1. **Guest checkout**

The guest checkout form is must for all online stores for the customers who don’t want to have an account.

To enable the Guest checkout, go to J2Store &gt; Setup &gt; Configuration &gt; Cart tabSet **YES** to Allow guest checkoutSave. 

![Easy-checkout-guest-checkout](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-guest.png)

**2. New account registration**

To enable the New account registration option in Easy checkout,

Go to J2Store &gt; Setup &gt; Configuration &gt; Cart tabSet YES to Allow quick new user registrationSave.

If new user registration option is enabled, you would see the small checkbox labelled **Create an account for later usage** in the checkbox.

This checkbox will be checked automatically.

 If customers don’t want to register, they can uncheck the checkbox and proceed further as a guest \(Non-registered\).

![Easy checkout-allowing new user registration](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-allow-user-registration-frontend.png)

![Easy checkout create a new account checkbox](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-unselectbox-creating-new-acc.png)

**3. Existing customers**

The existing customers can place the order by using the login form. You would see the login form by clicking on **Login**.

 

![Easy checkout login](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-login.png)

![Easy checkout login form](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-loginform.png)

**4. Checkout menu**

The SEF is the most important one for all the online stores. Similar to the Normal checkout, the easy checkout also has the menu item type.

By using this menu type, you can have the SEF url for checkout page.

Go to menu manager and create the menu item with type **Easy checkout &gt; Checkout**.

![Easy checkout menu](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-menu.png)

**Screenshots**  

![Easy checkout login form filled](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-loginform-filled.png)

![Easy checkout existing user logged in](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-existing-user.png)

**Easy checkout is not showing up:**

Even after installing, enabling and creating a menu for easy checkout, if it is not showing up on the storefront, then this might be a reason.

Navigate to\*\* Components-&gt;Easy checkout-&gt;Options\*\*

![Associating menu with easy checkout](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easy-checkout-associate-menu.png)

\*\*Select the menu created for easy checkout at the Easy checkout menu option.

![Choose the menu created for easy checkout](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easy-checkout-choose-menu.png)

  

![Enabling coupons and vouchers in easy checkout](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easy-checkout-enabling-coupons-vouchers.png)

![Frontend with coupons and vouchers enabled](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easy-checkout-coupons-vouchers-frontend.png)

![Easy checkout coupons and vouchers form](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easy-checkout-coupons-vouchers-clicked.png)

