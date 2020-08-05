# Royal Mail Shipping

The plugin integrates J2Store with the Royal Mail Shipping Rates API to get shipping price quotes in real time.

To use this plugin, your store must use GBP currency and your products needs to be set up with weights and shipping dimensions.

> This plugin primarily works with Centimeter\(cm\) and Gram\(g\).

**Features**

1. Choose what Royal Mail services you want to offer customers.
2. Add extra costs to services, if you wish.
3. Pack items individually or use our built-in box packer to ship items in single or multiple package\(s\).

**Installation**

1. Download Royalmail shipping plugin from our site and install it using Joomla installer.
2. After installing the plugin, go to J2Store &gt; Setup &gt; Shipping methods and enable RoyalMail Shipping for J2Store.
3. Once activated the plugin, open and configure it.

**Setup and Configuration** **Parcel packing method** There are two packing methods with Royal Mail; each affects the parcels you send to the plugin for a quote.

**Pack items individually** Each item in your cart will be sent to the plugin individually. Quotes for all items will be combined for the final cost.

**Box-Packing** The box packer included with this shipping method lets you group items into packages for which you define height, width, length, empty box weight and maximum box weight. The packing is mainly volume based, but does also consider item sizes.

**Services** This parameter controls the services and rates that you offer for your customers. Choose the services from the list of available services.

**Weight and Length unit** The weight unit must be Gram \(g\) and length unit must be Centimeter \(cm\).

**Tax Class** If you would like to charge tax for shipping, choose the tax profile here.

**GeoZone** Choose geo-zone and restrict the availability of this shipping method to the countries/zones in that geo zone. Choose All for making this shipping method available to customers from all regions.

**Handling Cost** If you would like to charge additional charge \(surcharge\) or handling fee, enter your cost of charge in number.

**Debug** Set YES to enable debug mode. Enabling debug mode will logged the debug messages in a file and saved in cache folder of your Joomla root directory.

DO NOT enable debug mode in live site.

![settings](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/royal-mail-shipping/royal-shipping-settings.png)

![product settings](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/royal-mail-shipping/royal-product-settings.png)

![shipping rates](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/royal-mail-shipping/royal-shipping-rates.png)

