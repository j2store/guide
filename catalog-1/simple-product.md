# Simple product

## Introduction <a id="introduction"></a>

A most common product type. It suits the requirements of most of the store owners.

You can create a simple product with or without product options. The inventory for this product type is managed for the primary product \(Not for the options\). All option types can be associated with the simple product.

 

![Simple product dashboard](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-dashboard.png)

## Creating a simple product <a id="creating-a-simple-product"></a>

Lets go through the available settings / fields for the simple product type.

### General <a id="general"></a>

The general tab has several fields, in which we need to enter the necessary and relevant details, attached with the product.

Have a look at the image below:

![Simple-product-general tab](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-general.png)

* Visible in Storefront - IMPORTANT: Set this to YES if you want this product to be shown in the storefront.
* SKU - Enter the SKU number of the product
* UPC/EAN/JAN/ISBN - Enter UPC/EAN/JAN/ISBN code for the product whichever is relevant. UPC - Universal Product Code \(In US/North America\) EAN - European Article Number \(Outside North America/Europe\) JAN - Japanese Article Number \(Only in Japan\)ISBN - International Standard Book Number \(Globally\)MPN - Manufacturer Part Number \(Globally\)
* Brand or Manufacturer - Select the brand or manufacturer of the product from the available list
* Vendor - Select the vendor from whom the product is available for purchase - Note: This feature is available in J2Store PRO version only
* Tax Profile - Specify whether the product is taxable and if so, select the tax profile relevant to the product
* Main Tag - The tag selected here will be used for canonical url. More details about canonical url could be found [here](http://docs.j2store.org/canonical-url-plugin)
* Cart Button Text - Enter the text to be displayed in the cart button
* Product css class - Use this option add unique css class to each product. 

### Pricing <a id="pricing"></a>

Add the price of your product. Depending on your requirement, you can also choose to configure an advanced pricing from here.

Now, check the image below:

 

![Pricing tab](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-pricing.png)

As illustrated in the image, you can set the regular price by entering the value in the text box. If you want advanced pricing, click the ’**Set Prices**’ button and it will open up a pop-up window to allow you to set an advanced price setting.

Let us see how it happens. Check the image below: 

![Advanced pricing](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-advanced-pricing.png)

* Select the dates \(optional\), between which you wish to set the advanced price. This option is not mandatory. For instance, you can offer a special price throughout the year, for a bulk purchase.
* Quantity range for this price to apply. This is also optional and if there is no minimum quantity required, just leave it as empty.
* Select the customer group to which you offer this special price. Default: Public
* Now enter the special price and click Create.

The price will be added and displayed below. You can edit that if you need, and click **Save all prices**.

If you want to remove that, you can do it by clicking the **Remove** button.

### Inventory <a id="inventory"></a>

* This is J2Store PRO exclusive feature \*

This tab has the configuration setup facility for inventory management. Here you can set the following details with respect to inventory. Check the image below:

 

![Simple product inventory](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-inventory.png)

From the image you can understand the following:

* Manage Stock - To enable Stock Management - Select Yes
* Stock Quantity - Enter the initial stock quantity
* Allow Backorders - Choose from the options whether or not to allow backorders to customers, i.e., the customer can order a product even if there is no stockAllow but notify customers - The second option would allow customer to purchase a product even if it is not in stock.A message will appear \(a notification\) before the price stating that: This item can be backordered.

This comes from the language file. The constant is: J2STORE\_BACKORDER\_NOTIFICATION

You can write a language override for this constant and display a customized message.

NOTE: This notification will display if:

* Stock is 0

This option is for those who sell fast moving products. So even if a product stock reaches 0, the customers could still order.

* Stock Status - Select stock status i.e., In stock or Out of stock
* Notify if stock goes below - Set minimum stock level for low stock alert
* Quantity Restriction - Choose whether purchase quantity is restricted and if Yes, set the limits for minimum and maximum quantity for a purchase by entering the quantities in the fields provided
* Use store configuration - If you select ‘Use store configuration’, you cannot enter max and min quantity fields, as they will be disabled

### Video Tutorial: <a id="video-tutorial"></a>

{% embed url="https://youtu.be/LLDVWW1FfdM" %}



### Images <a id="images"></a>

In this tab you can add images that can help the customer to understand more clearly, the product he wants to buy. Images help the prospect to imagine how the product intended to purchase will look like.

See the image below:

![Images](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-images.png)

Let us understand this with an example.

Lets assume that a customer would like to purchase a car. Now, car images need to be loaded in this tab.

* Main Image - The main image will be a general photo image of the car, that has to be uploaded by clicking on the ‘Select an image’ button and select the appropriate image from the files.
* Thumbnail Image - The thumbnail image would be something that represents the original product, but it would be a much smaller one to fit into a button, that will be shown up in the cart. By seeing this, the customer will understand that his product is displayed on the button and will click the button to see more details about the car.
* Additional Images - Additional images help the customer to know more details about the car, which will be showing the car view in many angles, and the customer will understand it clearly how it looks like, what the technical details of the car, the colour, and so on.

{% embed url="https://youtu.be/maTqM-vA2zU" %}



### Shipping <a id="shipping"></a>

This tab has the configuration setting for shipping. Any product that has been purchased, has to be shipped to the customer, if the product is physically deliverable.

Consider the image below:

 

![Shipping](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-shipping.png)

As shown in the image, you need to do the following activities to configure shipping:

* Enable Shipping - Select Yes to enable shipping
* Dimensions - Enter the dimensions of the packed product in Length x Width x Height
* Length Class - Choose a length class from the list e.g., cm, mm, inch, etc.
* Weight - Enter the net weight of the product when packed in the field provided
* Weight Class - Select the weight class from the list like Kg, grams, pounds, etc.

### Options <a id="options"></a>

In this tab, you can set your preferred options for a particular product like, colour of the product, size of the product, weight of product, mass of the product etc.

See the image on how to set the option for a product.

![Options](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-options.png)

Once you select the option from the dropdown list, it will be added as you can see in the image below.

![Adding options to product](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-add-options.png)

In the image, you have a text field to enter the option name like color, size etc. Just enter that in the text field. It will be set as preferred option.

If an option is created and set already, you can also import it here rather create a new option. Click the button and it will direct you to the predefined options, if any.

### Filters <a id="filters"></a>

Filters are certain attributes that help narrow the search of a particular product.

For e.g., assume that a customer searches for purple t-shirts in the store. Now, the productfilter is set as colour &gt; purple, to narrow the search. See the image below:

![Filters](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-filters.png)

Now the cart will display only the purple t-shirts.

### Relations <a id="relations"></a>

Relations are used to promote sales by suggesting the customer with higher value products than the one being looked and additional products to be bought with a particular product.

![Relations](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-relations.png)

* In this tab page, relations are set for Upsells and Cross sells
* An upsell is to get the customer to spend more money – buy a more expensive model of the same type of product considered for purchase.
* A cross-sell is to get the customer to spend more money buy adding more products from other categories, additionally, along with the product intended for purchase.
* Example:The terms cross-sell and upsell are often used interchangeably because, let’s face it, this gets confusing. Say the customer is viewing a Laptop with 2GB/500GB for $500.

You can suggest the customer with some options, so that the customer may be convinced to buy one of your options, thus promoting a higher sale for you.

Your suggestions could be like this:

* 4GB/500GB-&gt; $550 - Upsell, same product family, more expensive
* 4GB/1TB -&gt; $700 - Upsell, same product family, more expensive
* Laptop Bag -&gt; $25 - Cross sell, related product, additional sell

## App <a id="app"></a>

Custom fields / settings from applications will be displayed in this tab.

### A step-by-step guide to create a simple product <a id="a-step-by-step-guide-to-create-a-simple-product"></a>

**J2Store** implements an innovative concept in creating products. It uses the Joomla articles as products. So to create a product is to create an article.

So, lets create an article a.k.a a simple product

Creating an article / product

Have a look at the image below:

![Adding a new article](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-add-new-article.png)

As given in the above illustration, click in the top menu or in the left pane of the control panel. You will get a new screen like this.

![Save and proceed](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-save.png)

* Enter a name for the product you want to create.
* Select the ‘J2Store Cart’ tab below.
* Select ‘Yes’ in the option ‘Treat as product’.
* The next option is product type. From the available list, select ‘Simple’, as shown in the image.
* Now click the button, ‘save and continue’.

Your product will be saved, and it will continue to configure the product. See the image below: 

![Adding a content](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-add-content.png)

Now, add a description to your product in the editor. Lets add the other primary details of the product. See the image below.

 

![General tab](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-articlegeneral.png)

In general tab of the simple product, you can set up the basic information about the product like SKU, Universal Product Identifier, Brand etc and you can decide whether the product is to be displayed in store front. Next is pricing tab.

 

![Adding a pricing](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-articlepricing.png)

Here, enter the price of the product. If you want to set advanced prices, like special discounts, click the ‘Set Prices’ button ant you will get a pop-up window, where you can set the special prices. See image below to understand how it is done.

![Adding an advanced pricing](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simplepro-add-adv-pricing.png)

Enter the dates between which the special price is offered, the minimum quantity to avail the special price, the user group eligible, the special price and click ‘Create’. Now, the new price is listed as a row below. You can further edit and save or delete if you want. Lets move to Inventory, to understand stock management.

![Inventory](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-add-inventory.png)

_This is a J2Store PRO exclusive feature_

Select ‘Yes’ if you want inventory management. Enter all the fields as required. They are fairly self explanatory, still assisted in the image. And move on to images.

![Adding images](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-add-images.png)

Here, you can add the images for your product. The main product image, thumbnail image, and additional images for the product are added here. To add an image, click the green button, ‘Select an image’, which will bring up a pop-up window, where you can select the product image. See the image below: 

![Image upload](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-image-upload.png)

You need to load the image in the top window to select an image. To load an image, select the source by the browse button, up load it and insert it. Now, shipping. Check the image below:

![Shipping is enabled](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-enabling-shipping.png)

Enter the options with details according to your needs to enable shipping, the dimensions and weight of the product, classes for length and weight. Next is options.

![Options configuration](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-options-config.png)

You can add options for your product, as illustrated in the image. If you have already set an option for some other product, and wish to import the same option to this product, you can do so by clicking the import product options button, which will bring out a popup window, like this.

![Importing options on a simple product](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-options-import.png)

Next comes filters. You can filter the products, with their name or type to narrow the search. For e.g., if give ‘Electronics’ as filter, only electronics goods will be searched for your product, thus saving time. You can set filters as shown in the image.

![Adding filters to simple products](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-adding-filters.png)

The next tab is Relations. Here, you can add products of higher value than the one being viewed by the customer and recommend the customer to buy that product, citing its advantages and additional features. This is an upsell.

Refer the image below:

![Adding relations](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-adding-relations.png)

Also, you can add some other products to convince the customer to buy theses products additionally. This is cross sell. For more detailed explanation, refer to the **Relations** section of the **Simple Product**. The next tab is Apps.

 

![Apps section](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simple-pro-apps.png)

In this tab, you can add third party tools or plugins, that are available, to enhance the J2Store functionality, like adding additional fields, applications, functions or features.

Now, lets have a look on how your product is viewed in your online store. Check the image below:

![Simple product on frontend](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/simple-product/simpl-epro-frontend.png)

### Video Tutorials: <a id="video-tutorials"></a>

{% embed url="https://youtu.be/W8FvgG5vY-Y" %}

{% embed url="https://youtu.be/qCAg-auEoHg" %}



