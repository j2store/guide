# Zoo

**Introduction**

The plugin integrates Zoo content construction kit with J2Store, thus adding ecommerce capability to zoo.

**Requirements**

PHP 5.2 or higher Joomla 3.x J2Store 3 or above Zoo j2store_zoo_unzip_first\(Extract this package to get installation packages \)Item J2Store \( plg_itemjtwostore \)System Zoo J2Store \( plg_system_zooj2store \)

**Installation Instructions**

Note:When you download the Zoo Plugin You will have the package named “j2store_zoo_unzip\_first”, if you unzip the package you will find two zipped package .These two package are most important and need to be installed and to be enabled.

Unzip the Package “j2store_zoo_unzip_first.tar.gz” download from the site.Now, you will have two packages plg_itemjtwostore.tar.gz, plg_system_zooj2store.tar.gz. Use the Joomla Extension manager to install both the plugins one by one.

**Enable System Zoo J2Store Plugin**

Go to Extensions-&gt;Plugin Manager -&gt; Select the Plugin “System Zoo J2Store” and enable the System Plugin.

**Enable Item J2store in Zoo**

In the backend, go to Components -&gt; Zoo. Click on the Setting Icon.

 

![zoo1](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo1.png)

Let us say, you want to treat a Blog item as product. \(Zoo has a number of other content types as well. Blog content type is taken as an example \)

Edit the Blog -&gt; Article -&gt; Click Edit Elements

 

![zoo2](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo2.png)

![zoo3](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo3.png)



Here you can see **JTwoStore** element in the list. \(Numbers seems not working. That is why J2Store has become JTwoStore:-\) \)

![zoo4](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo4.png)

Now click on the element, you can see JTwoStore element added to the article element list\(see Left Side\).

 

![zoo5](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo5.png)

You have to enter the name of the element to display in the article item. Enter as J2Store as the name and Shopping cart as the description. Now save the changes.

Click on the new button -&gt; Click Article

![zoo6](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo6.png)

![zoo7](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo7.png)

Enter the Title to the article and other required fields .

![zoo08](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo8.png)

Enter the required fields and Save once. After successfully saved, you can see the Jtwostore Element added to your item.

![zoo9](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo9.png)

7.Now in Treat as Product, select **Yes -&gt;** select the type of the product

IMPORTANT: Click **Save**. Only then you can see the product related fields.

![z0010](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo10.png)

After save, you will able to see **J2Store cart** tab there and you can enter the details about the product.

Save changes.

**Frontend Customization Instructions**

In the backend, go to Components -&gt; Zoo, click on the Setting Icon on

![zoo11](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo11.png)

Now edit the Blog -&gt; Article - &gt; your template layout-&gt; click the Full layout

![zoo12](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo12.png)

Now you can see J2Store Cart in the layout list, you have to drag the J2storecart from the right to the left side in your desired area.

![zoo13](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo13.png)

![zoo14](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/Zoo/zoo14.png)

Save changes.

To see Cart at front end, create Zoo Menu Item for the Zoo Articles.

Click on the article that you have enabled as product, you can able to see J2store Cart.

