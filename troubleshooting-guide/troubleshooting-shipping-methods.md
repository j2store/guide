# Troubleshooting Shipping Issues

## Introduction <a href="#introduction" id="introduction"></a>

You have installed the shipping plugin but it doesn’t show up during the checkout. Here are a list of reasons that might be preventing the plugin from fetching shipping cost real-time from the APIs of the Shipping carrier.

## Common Issues <a href="#common-issues" id="common-issues"></a>

There are certain common issues that prevents the shipping methods from showing up in the checkout.

### Enable Shipping <a href="#enable-shipping" id="enable-shipping"></a>

Well. This might sound trivial. But some of us often forget to turn on the Enable shipping switch while creating the product. Make sure that Enable shipping is set to YES.

By default, Enable Shipping is set to NO. So this should be your first check.

![shipping enable](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-shipping-methods/shipping\_enable\_item.png)

### Geozone <a href="#geozone" id="geozone"></a>

All the plugins come with a geozone filter setting.

In Standard shipping methods, all the shipping rates are geozone specific. So you MUST configure the geozones correct before you set up the shipping cost.

![shipping geozone](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-shipping-methods/shipping\_geozone.jpg)

Geozones are nothing but a group of countries / zones.For example, shipping cost to a group of countries will be same. So those countries could be grouped to form a geozone.

Based on the shipping address provided by the customer, the system will look up for a shipping method and the rate and display it to the customer.

> NOTE If you ship your goods to the entire world and use shipping plugins like USPS, FedEx or UPS, you will have a param called: All geozones. Choosing this will allow the plugin to work for all shipping locations. Check the screenshot below

![geozone setting](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-shipping-methods/shipping\_geozone\_setting.png)

### Issues specific to standard shipping methods <a href="#issues-specific-to-standard-shipping-methods" id="issues-specific-to-standard-shipping-methods"></a>

J2Store comes with seven standard shipping methods built-in. The following are some of the common issues:

Shipping method configuration

1. The maximum sub-total and minimum sub-total condition does not match with your order-sub total. Check and make sure all the conditions you have in configuration page is correctly configured.
2. You have accidently disabled the shipping method. But looking for shipping option to be displayed at frontend.
3. Do you have weight based shipping method? But no shipping cost is showing ? The reason might be mismatching of weight range you have in Set rates and the weight of your product.
4. It seems to be caching so the rates are not get saved properly. Open your shipping rates and save it once again. Clear the cache and check.

### Set Rates <a href="#set-rates" id="set-rates"></a>

After creating a shipping method (by going to J2Store admin -> Set up -> Shipping -> Standard Shipping Methods), you can see a link named Set Rates. Click on it to set the shipping rates for the chosen shipping type.

## How Box Packing Works

Below mentioned is a common work flow on box packing with J2Store.

1. Finds boxes that fit items being packed (uses H x W x D).
2. Packs all items into boxes (using volume).
3. Uses the largest box fitting 100% of items _or_ uses the highest % packed box, and then passes unpacked items back (and repeats the process)
4. Packs unpackable items alone, using item dimensions.
5. Returns all packed boxes (parcels)
6. The plugin then sends the parcels to Fedex API
7. The API returns the rates with applicable shipping services
8. The returned shipping services and rates are shown to the customer

So according to box packing, dimensions is the primary factor and weight is the secondary one. Both the product dimensions and the Box dimensions entered by you on the shipping plugin would be considered and the products would be enclosed in the best suitable boxes.

### For Example&#x20;

Let us assume that you are using Fedex as your shipping carrier and setting up box packing.                When it comes to individual packing, the Fedex API requires item's dimensions and weight.\
**For example,**\
1\. Consider cart contains 3 items\
2\. Each item in your cart will be sent to Fedex.\
3\. Each item pack individually. Like,\
Item 1 => 3x4x5 and weight 10 = its a valid pack => pack 1\
Item 2 => 10x10x10 and weight 20 = its a valid pack => pack 2\
Item 3 => 5x5x5 and weight 4 = its a valid pack => pack 3                                                                                     4. Now Fedex would send the rate for the above packs.Please note that you should not sum up package weight as it would exceed the maximum limit according to Fedex rule.In box packing method, Fedex considers pre-defined box values (weight, width, length, height and max-weight) that you entered in the plugin but also considers item size.

## Issues specific to plugins like USPS, FedEx, UPS, CanadaPost, Australia Post <a href="#issues-specific-to-plugins-like-usps-fedex-ups-canadapost-australia-post" id="issues-specific-to-plugins-like-usps-fedex-ups-canadapost-australia-post"></a>

Shipping carriers have different limitations in the methods offered by them. For example, UPS only accepts Pound / Inch, Kilogram / Centimetre as the weight / dimension combination. A change in this would result in an error and no methods will be shown.

The following are common issues which affect the display of shipping methods.

### Weight and Dimensions <a href="#weight-and-dimensions" id="weight-and-dimensions"></a>

All the shipping carriers use the weight and the dimension of your product (Length, Width & Height) of your products ) to calculate the shipping cost (besides using the destination address). So make sure that you enter the Weight and the dimension of your product.

You should select the weight and the length measurement unit from the drop down list.

&#x20;Also make sure that you choose the correct measurement units in the plugin settings as well. If the measurement units used in the products does not match with the settings in the plugin, then J2Store will attempt to convert the values to the measurement unit set in the plugin.

![weight and dimensions](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-shipping-methods/weight\_and\_dimensions.png)

### API credentials <a href="#api-credentials" id="api-credentials"></a>

All shipping carriers have a web service and provide credentials to access their Rate API. Some of the carriers like USPS offer TEST accounts as well. Make sure you enter these credentials correctly in the Plugin. Some of the carriers provide Customer number (like Canada Post ) and a few other parameters as well. Refer the documentation PDF that come with each plugin for more information.

### Currency <a href="#currency" id="currency"></a>

In USPS shipping plugin, if the shipping server is queried, the server will return the list of options and their corresponding rates in US$. The shipping plugin may not show the rates if USD is not present in your list of currencies and you have configured a currency other than the US $, like CAD or AUD. To avoid this issue, you must have USD as a currency in your list of currencies. This will solve the issue.

### UPS accepted measurements <a href="#ups-accepted-measurements" id="ups-accepted-measurements"></a>

Only KG (Kilogram) and LB (Pound) are supported by UPS as the weight measurement units. Similarly, only IN (Inch) and CM (Centimetres) are supported as length measurement units.

And there is more. If you use Pound (LB) as the weight measurement, then the length measurement should be Inch (IN). Similar if KG is used, then CM should be the measurement. A wrong combination will result in an error.

### Debug Mode <a href="#debug-mode" id="debug-mode"></a>

In your plugin settings, set the Debug mode to YES. This will allow the plugin to log the responses sent by the APIs of the shipping carriers.

The log is stored in the /cache folder of your Joomla Root. You can use your Hosting CPanel’s file manager or an FTP program like FileZilla to access the log file. The log should give you a lot of information.

VERY IMPORTANT: Debug mode SHOULD NOT be enabled in LIVE / PRODUCTION sites.&#x20;

![debug mode](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-shipping-methods/debug\_mode.png)

Still not working, please create a private ticket or email us the log file. We will help you troubleshoot.
