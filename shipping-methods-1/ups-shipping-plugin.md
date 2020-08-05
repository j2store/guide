# UPS Shipping Plugin

This plugin integrates UPS Shipping Rate API with J2Store.

**Requirements**

* PHP 5.3+
* Joomla 2.5 / 3.x +
* J2Store 2.6.8 +

**Installation** You can install the plugin through the standard Joomla installer.

**Configuration** Prior to configuring the plugin, you should have an active account with the UPS and received API keys. Contact UPS to register and get API keys.

Not sure where to find your Access key ? Read the documentation below &lt;link-text url = ¨[https://help.extensionworks.com/hc/en-us/articles/200366638-Where-do-I-find-my-UPS-license-key-or-Access-Key-”target](https://help.extensionworks.com/hc/en-us/articles/200366638-Where-do-I-find-my-UPS-license-key-or-Access-Key-%22target) = ¨\_blank”rel = ¨noopener¨&gt; click here

Refer the image below:

![ups1](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/ups-shipping-plugin/UPS1.png)

**Access Key** Enter the access key provided by the UPS.Not sure where to find your Access key ? Read the documentation belowhttps://help.extensionworks.com/hc/en-us/articles/200366638-Where-do-I-find-my-UPS-license-key-or-Access-Key-”target = ¨\_blank”rel = ¨noopener¨&gt; click here

**Username** Enter your UPS username.

**Password** Enter your UPS password.

**Shipper Number** This is actually the shipping account number provided by the UPS.

**Parcel Packing Method** UPS will provide 2 types of parcel packing methods.

* Items Individually
* Box Packing

**Items Individually** Each product considers as a separate unit and packing it into the individual boxes. Each product will be packed separately.

**Box Packing** The box packing included with this shipping method lets you group items into packages for which you have to define height, width, length, weight and max weight. Packing is mainly volume based but also considers item size.

**UPS Packaging Box** UPS Packing box offers more box packing tyoe which are listed here. You have to choose/select more than one option from the list.

* UPS Tube UPS tube accommodates and protects larger documents which should be rolled rather than folded. Use the tube for blueprints, charts, maps, drawings, or posters. Charges are based on the billable weight and zone.

Triangular tube for rolled papers; 38in x 6in x 6in \(96.5cm x 15cm x 15cm\)

* UPS Pak UPS Pak accommodates Padded, secure, or watertight boxes for sensitive or regulated items; size varies.
* Ups Express Box - Small The maximum size of the box is 13in x 11in x 2in.
* UPS Express Box - Medium: The maximum size of the UPS Express box is 16in x 11in x 3in.
* UPS Express Box - Large: The maximum size and weight of the box are 18in x 13in x 3in and weight limit 30lbs.
* UPS 10 KG Box: The maximum size and weight of the UPS 10 kg box are 16.5in x 13.25in x 10.75in \(42cm x 34cm x 27cm\); weight limit 22lbs/10kg.
* UPS 25 KG Box: The maximum size and weight limit of the UPS 25 kg box is 19.75in x 17.75in x 13.25in \(50cm x 45cm x 34cm\); weight limit 55lbs/25kg

**Box List** If you choose box making then you have to define/set box size. The box will have the following fields.

1. Name: This allows you to name your custom packages. This name will show in the Debug if that package is used.
2. L \(in\), W \(in\), H \(in\): The first set of dimensions are the outer dimensions of the package. These are the dimensions passed to the API. If you are working with a flat rate box via the API \(i.e., Regional Boxes\), use the API’s ‘inner dimensions’ for your box’s outer dimensions. Your box must ‘fit’ inside.
3. Inner L \(in\), Inner W \(in\), Inner H \(in\): The second set of dimensions are for the inner dimensions of the packaging. This should be the outer dimensions minus the thickness of the package walls. These dimensions are used for packing and items must fit within them \(they cannot be the same size as the products, allow for a little extra room\).
4. Weight of Box \(lbs\): This is the weight of the empty box by itself. This weight is added to the total weight of the contents.
5. Max Weight \(lbs\): This is the maximum weight your box can hold. This includes the weight of the box and the contents.

**Handling Cost** If you need to charge a handling cost for the shipping, you can enter here.

**Test mode** If you would like to use the UPS in test mode then set this option to ‘yes’ otherwise set the test mode as ‘no.

**Delivery Confirmation Option** UPS will provide confirmation of delivery without the recipient’s signature.

There are 2 options available

1. Signature Required
2. Adult Signature Required
3. Signature Required :UPS will obtain the recipient’s signature and provide you with a printed copy. You may also view the recipient’s signature online.
4. Adult Signature Required :UPS will obtain the adult recipient’s signature and provide you with a printed copy. You may also view the adult recipient’s signature online.

**Direct Delivery Only** Direct Delivery Only ensures a package is delivered to the residential or commercial address you provide.It does not require the signature. If you set ist ‘yes’ means direct delivery gets enabled. If you set it as no means direct delivery does not get activated.

**Services** Choose the shipping services that you would like to provide to the customers.

> NOTE: Services depend on the customer’s shipping address. Even if you chose many services here, UPS will show only the services that are available to the customer’s shippingdestination at the checkout.

**Pickup Type** Choose your Pickup type.

**Packaging** Choose your packaging option. Default: Package

**Customer classification** Wholesale - If you are billing to a UPS account and have adaily UPS pickup, Occasional - If you do not have a UPS account or you are billing to a UPS account but do not have a daily pickup, Retail - If you are shipping from a retail outlet \(onlyused when the origin is the US\).

**Weight Unit** Valid Units are Kilogram \(KGS\), Pound \(LBS\).

> IMPORTANT: You must choose a weight unit here. Otherwise, the plugin will not work. If you are using more than one weight unit for your products, then the plugin will automatically convert to the weight unit you are choosing here.
>
> ExampleProduct A – Weight is 5 KG , Product B – Weight 7 Pounds.

You have set the Pound as the weight unit in the plugin params.Then the Product A weight will be converted to pound, according to the values provided at the Weight Classes section \(J2Store admin –&gt; set up –&gt; weight classes\).

**Show Weight Total** Set this to yes to show the total weight of the products in theorder to the customer during the checkout. The weight will appear next to the shipping method name.

**Length Unit** The length unit. The plugin will not convert the length unit. Make sure that you are using the same length unit for all your products.

**Tax Class** If you want to charge tax for shipping cost, choose a tax class here. Otherwise, leave this field empty / do not select any option.

**Geozone** You can select a geo-zone and restrict the availability of this shipping method to the countries/zones in that geo zone. Leave empty / unselected for making this shipping method available to customers from all regions.

**Debug** If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory.

Refer the below image

![ups2](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/ups-shipping-plugin/UPS2.png)

