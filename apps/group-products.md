# Group Products

This app allows store owner to combine the products and sell it as one group product. When grouping product, the app will allow only simple, configurable and downloadable product types without options. Product which are having options can’t be added into the group.

**Requirements**

* PHP 5.4 or higher
* Joomla 3.3 or above
* J2Store 3.2.x or above

**Installation**

1. Use the joomla installer ot install the app.
2. Go to J2Store &gt; Apps, find the Group Products app and click enable to activate the app.
3. Once enabled, you dont need to configure anything in the app. Just go to article manager and click new article.

**Group Products**

1. Once you enabled the app, you can see Group Products as one of the product types listed in the product type dropdown. Refer the picture below
2. Select the product type Group Products and click save.
3. Go to J2Store cart and scroll down where you can see the navigation menus \(General, images,Relations,apps\)
4. In general tab, choose YES to visible in storefront and navigate to apps.
5. Go to apps tab where you can see the search box to search for the products.
6. Type two or three characters of your product.
7. If the product you are searching for is not listed, the reason is that the product might have options. Since this app allows only the product without options, the product with options cannot be added into the group.
8. Once the products are added, save article and check in the frontend. 

![gp05](https://raw.githubusercontent.com/j2store/doc-images/master/apps/groupproduct_05.png)

**Usecase**

Let’s imagine the scenario, where you own a online book store and you wish to sell both the physical book and the digital copy of the book, then grouped products could be a boon to you.

Grouped product comes handy especially when you don’t want the user to go searching for the physical book in two different places and when you wish to allow the buyer to choose whether to buy the physical product or the digital copy of the product.Now, let us get to know how to create a grouped product for the above scenario.

Procedure to be followed

* Create a simple product, for the physical product, specifying the images, price, discount, stock information if any.
* Create a downloadable product, for the digital product, mentioning the product price, file to be downloaded after purchase, download limit and link expiry limit and so on.
* Create a product of the type “Grouped product”.
* Navigate to the Apps section and you will find the option to add other products to the group.
* Add the products that you wish to group into a bundle and save the article.
* Associate the grouped product to a category and link that category to a menu.
* Now the grouped product will be available at the frontend.

**Video Tutorial**

You can watch the video tutorial for Group Product app

{% embed url="https://www.youtube.com/watch?v=BNwL6AZ8eKA&feature=youtu.be" %}



