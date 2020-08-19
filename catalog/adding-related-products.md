# Adding related products

Adding related products has never been as easy as it is now. Here is how you could add up-sell and cross-sells products on your store.

### Scenario: <a id="scenario"></a>

Let us suppose your site sells Tea cups, Tea pots and Serving plate. Let us suppose that the product Brook Ceramic serving plate from the serving plates section is related products to another product named Paragon Blue Tea cup from the Tea cups section and you wish to see the Hand painted Tea pot from the Tea pots menu in the cross-sells section.

### Steps to be done: <a id="steps-to-be-done"></a>

* Create an article for Paragon Blue Teacup.
* Create another article for Brook Ceramic Serving plate and one for the hand painted tea pot.
* In the relations tab of Paragon Blue Teacup article, and type in Brook Ceramic Serving plate. 
* The Serving plate’s article would pop up. Add it to the up-sells section.
*  Now type the name Hand painted Teapot in the cross-sells section.
* The article with the name Hand painted Teapot would pop up. Add it to the cross-sells section.
* Navigate to menu manager-&gt;Create a menu for Teacups of the type J2Store-&gt;Product list.
* Navigate to the **Item view options** tab and set the options **Up sells\(Related products\)** and **Cross sells\(Related products\)** to **Yes**.
* Visit the frontend of the site and click on the Teacups menu.
* Now from the list of products displayed, click on the Paragon Blue Teacup.
* In the item view page of the Tea cup, the Serving plate would be listed in the Related products section.
* The Hand painted Tea pot would be available in the cross-sells section.

### Screenshots: <a id="screenshots"></a>

  

![Adding related products to Product](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/addingrelatedproducts-to-pro.png)

![Menu settings](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/addingrelatedproducts-menu-settings.png)

![Frontend view](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/frontendrelatedproducts.png)

### Video Tutorial: <a id="video-tutorial"></a>

{% embed url="https://youtu.be/X4QtLzaBPI0" %}

#### Showing related products on the cart page: <a id="showing-related-products-on-the-cart-page"></a>

By default, the related products would be displayed on the item view page of the parent product only.

Now that we have added the related products to the required parent products, we might want to display these related products on the cart page as well.

### How this module works: <a id="how-this-module-works"></a>

Once you have added related products to your parent products, all you have to do is, install the module, assign it to the pages you wish to display the related products and set a position where the module has to be displayed on the chosen pages.

**NOTE: Related products module would display the related products only if the product present in the cart has associated Relations to it. That is the product in the cart should have a related product added to it.**

### Installation: <a id="installation"></a>

* Download the module from the above link and install it through the default Joomla installer\(under Extensions-&gt;Install\).
* Navigate to Extensions-&gt;Modules-&gt;Edit the related products module.

### Configuration: <a id="configuration"></a>

The module has a number of options that allow you to customize the view of the module on the storefront.

![Related product module settings](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/rel-pro-mod-settings.png)

Once the layout configuration is done, now navigate to the Menu assignment tab on the module and choose the pages where the module should be published: 

![Module assignment](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/module-assignment.png)

 

![Position assignment](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/position-assignment.png)

![Related product module frontend](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/rel-pro-mod-frontend.png)

## Adding related product in the Joomla article view: <a id="adding-related-product-in-the-joomla-article-view"></a>

The related products in the article view has to be done with the help of [shortcodes.](http://docs.j2store.org/catalog/short-codes)

### Scenario: <a id="scenario-1"></a>

The product Net has to be added as a related product to the product Basket ball. The product id of the product basket ball is 17 and the product id of the product Net is 18.

### Steps to be done: <a id="steps-to-be-done-1"></a>

* Navigate to the J2Store cart tab and add the child product in upsell or crosssell field of the relations tab 
* Navigate to the product article of Basket ball-&gt;J2Store cart tab-&gt;Copy the shortcode **{j2store}17\|cart{/j2store}**
* Paste it in the content part and copy the shortcode for displaying the crosssell and upsell product and paste it in the content part of the parent product. The shortcode to be copied is **{j2store}17\|upsells\|crosssells{/j2store}**

![Shortcodes](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/rel-pro-addding-content.png)

* Navigate to the article of the related product-&gt;J2Store cart tab-&gt;copy the shortcode to display the product’s add to cart **{j2store}18\|cart{/j2store}**
* Paste the shortcode at the content tab

![Cart shortcode](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/cart-shortcode.png)

![Item view settings](https://raw.githubusercontent.com/j2store/doc-images/master//catalog/adding-related-products/content-plugin-item-view.png)

### Frontend display <a id="frontend-display"></a>

![Item view settings](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/content-plugin-item-view.png)

![Parent product on frontend](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/frontend-parent-pro.png)

![Front view](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/adding-related-products/rel-pro-view-front.png)

**VERY IMPORTANT NOTE: The above approach would work only if you have all of your products displayed in the Joomla article view and not in the J2Store list or tag view layout.**

You will have to insert the add to cart shortcodes for the other products, if not the add to cart button wouldn’t show up. 

