# Quantity dropdown

This app allows your store to update the price of a product based on quantity in the product page itself. Your product page normally displays the price for a unit quantity of a product. When a customer selects a higher quantity of the product, he can view the total price of the product only in his cart. But with this app he can automatically view the updated price for a higher quantity of the product in the same product page.

**Requirements**

* PHP 5.4 or higher
* Joomla 3.x or higher
* J2Store 3.2.10 or higher

**Installation**

1. Download Quantity dropdown from our site and install it using Joomla installer.
2. After installing the app, go to J2Store &gt; Apps and find Quantity Dropdown app.
3. Click on Enable to activate the app.
4. Click on Open to configure basic settings of the app.

**Configuration**

**Enable price update on quantity change to all products?**

Set this option to **YES** will enable the dropdown quantity box for all products.

**Quantity box type?**

Choose the type of quantity box to be displayed. There are two types of quantity box offered by this app: Dropdown and Default. The Dropdown type would display the quantity box in a dropdown format and the Default type would display quantity box in a J2Store’s normal quantity field format.

**Pre-defined quantity \(in a comma seperated format\)**

The quantity dropdown would render the quantity values entered here. You could enter the values in a comma \(,\) separated format. For example: 10,20,30,40,50

**Should a placeholder —Select— text be displayed instead of defaulting to the first option?** Choose this if you would like to force the customer to choose a quantity in the dropdown.

**Restrict the display of the dropdown to selected user groups?**

You could restrict the display of quantity box based on user groups. The quantity box would be visible to the users belong to the usergroup selected here.

**Enable using a Factor ?**

Set this option to YES if you would like to generate a quantity list using a factor \(example: 5. This should create a list of quantity in the increments of 5: example. 5,10,15,20\)

**Quantity Factor**

If you have enabled the above option, then you will have to mention the factor here. For example: Enter 5.

**Maximum limit for the quantity list when factor is used**

The maximum quantity should be mentioned here. For example: Enter 50. Now the quantity list will be 5, 10, 15, 20, 25, 30, 35, 40, 45, 50.

\*\*Multiply Price based on Qty? \*\*

Set this option to YES would display price with multiply of quantity. For example, consider the price of the product is 12. So when you change the quantity to 5 then it would display 60.

\*\*Enable cart quantity \*\*

If you would like to replace quantity box in items table on cart page with quantity dropdown, set this option to YES.

\*\*Quantity pre text and post text \*\*

Text entered here will be added as prefix and suffix to the quantity number. For example, if you entered Gram in the Post text box then the quantity will be appeared like 5 gram, 10 gram, 15 gram, etc..

![qd01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/Quantity%20dropdown/qd_01.png)

**Configuring Quantity dropdown at product level**

To configure quantity dropdown at product level, go to Article manager -&gt; Open the product -&gt; J2Store cart tab -&gt; Apps where you should enable Product quantity dropbox.

\*\*Override App settings for this products ? \*\*

If you wants the specific product to not use the app’s global settings, then set YES to this option. Choosing YES would not take the settings you configured at app. It would consider the settings configured at the product.

**Quantity box type?**

Choose Quantity box display type from the options\(Dropbox, Default\) available.

Dropbox : Choosing this option will display quantity box in dropdown type. Default : Choosing this option will display default quantity box.

**Pre-defined quantity \(in a comma seperated format\)** The quantity dropdown would render the quantity values entered here. You could enter the values in a comma \(,\) separated format. For example: 10,20,30,40,50

**Restrict the display of the dropdown to selected user groups?**

You could restrict the display of quantity box based on user groups. The quantity box would be visible to the users belong to the usergroup selected here.

**Enable using a Factor ?**

Set this option to YES if you would like to generate a quantity list using a factor \(example: 5. This should create a list of quantity in the increments of 5: example. 5,10,15,20\)

**Quantity Factor**

If you have enabled the above option, then you will have to mention the factor here. For example: Enter 5.

**Maximum limit for the quantity list when factor is used**

The maximum quantity should be mentioned here. For example: Enter 50. Now the quantity list will be 5, 10, 15, 20, 25, 30, 35, 40, 45, 50.

\*\*Quantity pre text and post text \*\*

Text entered here will be added as prefix and suffix to the quantity number. For example, if you entered Gram in the Post text box then the quantity will be appeared like 5 gram, 10 gram, 15 gram, etc..

![qd02](https://raw.githubusercontent.com/j2store/doc-images/master/apps/Quantity%20dropdown/qd_02.png)

**Frontend Demo Screenshots** 

![qd04](https://raw.githubusercontent.com/j2store/doc-images/master/apps/Quantity%20dropdown/qd_04.png)

**Support**

Still have questions? You can post in our support forum: [http://j2store.org/forum/index.html](http://j2store.org/forum/index.html)

Thank you for using our extension.

