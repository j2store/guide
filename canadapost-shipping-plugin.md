# Canadapost shipping plugin

**Requirements**

1. PHP 5.3+
2. Joomla 2.5 / 3.x +
3. J2Store 2.6.8 +
4. cURL

**Installation** You can install the plugin through the standard Joomla installer.

How to Register with Canada Post ?Sign in or Sign up If you are lready registered with Canada Post, then Sign in to the Canada Post website using your registered Username and Password.

Don’t have an account yet ? Sign up now.

**Join the Developer Program** Once you’ve signed in to our website, select Join Now on the main Developr program page. Read and accept the terms and conditions of the Program to become a member.

**Get your API keys** You would see the API keys that are displayed on the main Developer Program page. These API keys are unique codes, used to access Canada Post web service and Postmen API. Note down the API keys \(one for development and one for production\).

**Configuration** Prior to configuring the plugin, you should have an active account with the CanadaPost and received API keys. Contact CanadaPost to register and get API keys.

1. Make sure that you have set the Default Weight Class to Kilogram \(KG\) or Pound \(LB\) in the J2Store admin –&gt; Set up –&gt; Store Profiles –&gt; Your Store profile
2. Make sure that you entered your Postal Code/Zip correct in your Store Profile
3. Make sure that you have set the Dimensions and Weight fields in your products correctly
4. Make sure that you have set the Enable Shipping to YES in your products
5. Open the Canada Shipping Plugin and set the Following Parameters

**API Username** Your CanadaPost username

**API Password** Your CanadaPost password

**Customer Number** The customer number provided by the CanadaPost.

**CanadaPost Service** Choose the services provided by CanadaPost to display in checkout.

> NOTE: This is a mandatory option for version 3.2.24.Not selecting the service will make the shipping method unavailable.

**Handling cost** You can enter an amount here \(without any symbols or letters\). It will be added as a handling cost in addition to the shipping cost.

**Show delivery time** Set this to Yes, if you want to show the expected delivery time to the customers.

**Test mode** If you would like to test the API, set this to Yes. Otherwise, you can set this to No.

**Weight Unit** Valid Units are: Kilogram \(KG\), Pound \(LB\).

> IMPORTANTMake sure to set your default weight class to either KG or LB in your storeprofile. All your products should be using the same weight class

**Length Unit** The length unit. The plugin will not convert the length unit. Make sure that you are using the same length unit for all your products.

**Tax Class** If you want to charge tax for shipping cost, choose a tax class here. Otherwise, leave this field empty/donot select any option.

**Geozone** You can select a geozone and restrict the availability of this shipping method to the countries/zones in that geozone. Leave empty/unselected for making this shipping method available to customers from all regions.

**Debug** If you set this to Yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory.Set this to No in Live websites.

**Support** You can post your questions, if any, in [http://j2store.org/forum/index.html](http://j2store.org/forum/index.html).

