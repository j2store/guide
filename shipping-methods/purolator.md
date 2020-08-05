# Purolator

This plugin integrates Purolator shipping API with J2Store Joomla eCommerce solution.

**Requirements**

1. PHP 5.4 or higher
2. Joomla 3.x and above
3. J2Store 3.2.10 or higher

**Installation**

* Download the Purolator shipping plugin from our site and install it using Joomla installer.
* In Joomla backend, go to J2Store &gt; Setup &gt; Shipping methods
* Enable and open the Purolator shipping plugin to configure the basic settings.

![purlt](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/purolator/purolator_04.png)

**Basic Settings**

**API key:** Enter the valid API key provided by Purolator shipping.

**API password:** Enter your Purolator shipping account’s password.

**API account:** Enter the account number associated with your purolator account.

**Origin zip code:** Enter the postal code from where the shipping is actually made.

![purolator](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/purolator/purolator_01.jpg)

**Sandbox:** Purolator shipping offers sandbox feature to use the shipping in test mode. Choose YES will enable the sandbox feature.

**Box List:** Purolator Shipping comes with box packing feature. The box packing included with this shipping method lets you pack all the items into single box for which you have to define height, width, length, weight and max-weight.

**Purolator Service:** Choose the shipping services that you would like to provide to the customers.

> NOTE: Services are depend on the customer’s shipping address. Even if you choose many services here, Purolator will show only the services that are available to the customer’s shipping destination at the checkout.

**Handling Fee:** If you would like to charge handling fee, you can enter the amount here.

**Length unit:** The valid length units are centimetre and inch. Make sure that you are using the same length unit for all your products.

**Weight unit:** The valid weight units are kilogram and pound. Make sure that you are using the same length unit for all your products.

**Display delivery date:** Choosing YES will display the delivery date.

**Tax class:** Choose your shipping has to be taxable or not. If you would like to make your shipping taxable, you can choose your tax profile here.

**Geozone:** You can select a geo-zone and restrict the availability of this shipping method to the countries/zones in that geo zone. Choose All to make this shipping method available to customers from all regions.

**Debug:** If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory.

![purolator2](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/purolator/purolator_02.jpg)

![purolator3](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/purolator/purolator_03.jpg)

