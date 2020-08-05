# GeoIP Product Rules

Geo IP restricts helps you restrict customers from a certain geographical region from purchasing your products. With this app you can restrict purchase in two ways. You can block products from being viewed on certain regions. Or you can display a customised message that informs the customer that product is not available in his gepgraphical area.

**Requirements**

PHP 5.4 or higher Joomla 3.x J2Store 3.2.14 or higher Akeeba Geoip provider plugin

**Installation**

Before installing the app, you must install the Akeeba geo ip provider plugin to find the location of the customer using IP address. Download the Akeeba geo ip provider plugin from here [https://www.akeebabackup.com/download/akgeoip.html](https://www.akeebabackup.com/download/akgeoip.html)

![gpr01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/geoip-product-rules/gpr_01.png)

![gpr02](https://raw.githubusercontent.com/j2store/doc-images/master/apps/geoip-product-rules/gpr_02.png)

After finish Installing Akeeba Geopip provider, download the Geo IP Restricts app from our site’s extensions section. Once downloaded, you must extract the downloaded package and you will be having two zip files.

Install them one by one using Joomla installer.

Go to J2Store &gt; Dashboard &gt; Apps and enable the Geo IP Restricts app.

![gpr\_03](https://raw.githubusercontent.com/j2store/doc-images/master/apps/geoip-product-rules/gpr_03.png)

Now go to Extensions &gt; Plugins and choose search type **System** and enable System - Akeeba GeoIP provider plugin and System - Geoproducts plugin.

![gpr04](https://raw.githubusercontent.com/j2store/doc-images/master/apps/geoip-product-rules/gpr_04.png)

**Configuration**

**Step-1** Go to J2Store &gt; Dashboard &gt; Apps and open the Geo IP Restricts app

![gpr05](https://raw.githubusercontent.com/j2store/doc-images/master/apps/geoip-product-rules/gpr_05.png)

**Step-2** On opening the app, you will be having the following options:Function type: Here you have to choose the functional type of app. Choosing NO will hide the product visibility to the countries selected. Choosing YES will make the product visible to the countries you selected.

**Hide the product for countries in the selected geozones:** This option is used to choose which part of the product should be hidden in store front. You can hide either entire product or hide only the add to cart button. There is one more option in the dropdown which will show the entire product but block the cart function\(customer from the selected country cannot add the item into the cart\).

 

![gpr06](https://raw.githubusercontent.com/j2store/doc-images/master/apps/geoip-product-rules/gpr_06.png)

**Step-3**

* Now Go to Article manager and open / edit your product.
* Move to J2Store cart tab and navigate to Apps tab.
* Choose the customer’s country to which the product should be hidden/visible.

NOTE: You should create geozone for the country in J2Store -&gt; Localization -&gt; Geozones Frontend demo

If customer comes from US, add to cart button has been hidden. 

