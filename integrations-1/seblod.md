# Seblod

### Introduction <a id="introduction"></a>

The plugin integrates Seblod content construction kit with J2Store, thus adding ecommerce capability to Seblod.

#### Requirements <a id="requirements"></a>

* PHP 5.2 or higher
* Joomla 3.x
* J2Store 3 or above
* Seblod 3.x
* Plguin plg_cck_field\_j2store

#### Installation Instructions <a id="installation-instructions"></a>

Use the Joomla Extension manager to install the plugin.

* [**Configure J2Store in admin**]()
* [**Show J2Store content in Front-end**]()

## Configure J2Store in admin <a id="configure-j2store-in-admin"></a>

In this section, you will see how to create a SEBLOD article in the backend and frontend.

#### Adding J2Store Field <a id="adding-j2store-field"></a>

1. In the backend, go to Components -&gt; SEBLOD 3.x, as shown in the image below: 

![step 1](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/step-1.png)



2. Click on the icon **Forms & Content Type**. Click on the admin menu link **Construction** then **Forms & Content Types**.

 

![Step 2](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/step-4.png)



3. In the **Form & Content Type Manager**, you should click on the item **Article**. 

![Step 3](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/step-5.png)

4. Now we have to add j2store custom field to the **Article** content type, click on the ”+” \(button is placed at the right of the **Contruction** block\). A Form in window popup appears. 

![Step 4](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/step-6.png)

5. To add a **Text** field to an **Article** content type:

 

![Step 5](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/step-7.png)

6. Choose App Folder **Quick Folder**: then choose type **J2store** field. 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/create-article-step-3.png)

7. Save the changes. Now J2store field will appear under the Fulltext field \(at the bottom of your form on the first tab\).

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/create-article-step-4.png)

8. Save and close the article.

9. Go to the menu, **Content** -&gt; **Article Manager** -&gt; **Add New Article**. You will get the screen as shown below:

  

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/add-new-article-1.png)

Now scroll down. You will see the integrated j2store product type as shown below: 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/add-new-article-2.png)

10. The J2Store element appears at the bottom because, it is placed below the End of the Tab in the construction layout. So we need to rearrange the element to appear in the tabs. Consider the below image:

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/rearrange-j2store-element.png)

11. We need to add the J2Store element in the tab. To create a tab panel, click on the + sign in the right side and follow the procedure as shown in the image:

  

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/create-tab-panel.png)

In the above image, enter the details as shown and click **Save & Close**. The tab panel will be created. You need to rearrange the tab, as shown below:

  

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/replace-j2storetab.png)

By clicking on the rounded icon, you can confirm the tab panel details and close it.

12. Now, add a new product. You will see the screen like this: 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/create-new-product.png)

13. Now you can Configure your product, Set **Yes** for Visible in store to view at frontend. 

![Step 11](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/step-12.png)

### Product Creation in Front end <a id="product-creation-in-front-end"></a>

1. To create the product in the frontend, follow the procedure, illustrated with the help of images. In the Control Panel menu, go to **Construction** -&gt; **Forms & Content Types** 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/show-in-frontend-1.png)

2. Now, from the resulting screen, choose **Article** as shown below: 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/show-in-frontend-2.png)

3. Click on the **Site Form** as shown in the image below:

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/show-in-frontend-3.png)

4. In the right hand side, click on the ’&lt;’ symbol, next to the **J2Store Tab** and it will be added to the form as shown in the below image.

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/show-in-frontend-5.png)

5. After that, in the right side, near the ’+’ sign, choose ‘All App Folders’ in the select list and you can see a list of items displayed below. Scroll down to locate **J2Store\_Cart** and add it to the construction layout, by cliking in the ’&lt;’ arrow seen in the extreme right of the item. All these actions are illustrated in the image below:

  

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/show-in-frontend-6.png)

Place the **J2Store Tab** and **J2Store\_Cart** items in the positions, as depicted in the image by drag and drop.

6. Go to Joomla admin Control panel -&gt; Menus -&gt; Menu Manager -&gt; Add New Menu

a.Enter the Menu Title.

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-new-menu-item-0.png)

 b.Choose the Menu Item type **SEBLOD** -&gt; choose **Forms**. 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-new-menu-item-1.png)

 c.From **Content Type \(Form\)** input, select **Article** from the List. 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-new-menu-item-2.png)

 d. Save the changes.

7. In control panel, go to **Construction -&gt; Forms & Content Types** and click on **New**. In the resulting screen, enter the details as shown in the image below:

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/form-content-type-new-1.png)

8. You will get the screen like this, after you have rearranged J2Store Tab. Now, click **Save** 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/form-content-type-new-2.png)

9. Thats it. You have successfully created a SEBLOD article. You can choose it in the following ways.

I. Click on the **Add Content** as shown in the following image.

  

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/new-form-content-type-listed.png)

If you click on the **Add Content** you will get this pop-up window: 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/add-content-clicked.png)

 II. In main menu, go to **Content -&gt; Article Manager** and click on the **New** button as shown below:  

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/article-manager-list.png)

You will get the pop-up like this:

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/article-manager-list-new.png)

10. But before you add an article in this type, you need to do edit the article you have created further. Open it for editing.

  

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/edit-form-article.png)

Still you need to follow some more steps to complete the procedure. Arrange the items in the construction layout as shown in the image below:

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/form-article-final-setting.png)

11. Now, **Save** the page and create an article of type **Form\_Article** and you will have the product creation page like this:

  

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/form-article-new-product-details.png)

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/form-article-j2store-tab.png)



**The images below illustrates how to create a product in your frontend**

In your site frontend, you can see the newly created SEBLOD article, listed in the top right. See the image:

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/frontend-article-creation-1.png)

As shown in the image, click on the **New Article** and you will get the product creation page as shown in the next image. Enter a name for the new product and content for the product. This is **Contents** tab. Now, go to **J2Store** tab. Here, select **Yes** to _**Treat as a product**_ option and now click on **Save**.

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/frontend-article-creation-2.png)

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/frontend-article-creation-3.png)

Your product is created and you can configure the product with the product specific details, change the product type, set prices, etc.

## Show J2Store content in Front-end <a id="show-j2store-content-in-front-end"></a>

This section will help you understand how to display the SEBLOD article in front end.

The display can be achieved in the following methods:

* **Category Blog View**
* **Single Article View**
* **Search & List View**

To display SEBLOD articles in the frontend, you need to create a menu exclusively and then you can display it.

### Category Blog View <a id="category-blog-view"></a>

Before you proceed to view the article in frontend, you need to check one thing. Go to **Components -&gt; J2Store -&gt; Setup -&gt; Configuration**. Go to **Cart** tab. Now, check the setting of **Add to cart placement** option. Ensure it is selected with **Within article using tag** as shown in the image below. 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-cat-blog-cart-tab.png)

To achieve front end category blog view, we need to follow a few procedures as explained below:

In the backend main menu, go to **Menus -&gt; Main Menu**. You will get the **Main Menu Items** list, as shown in the image below:

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-menu-items.png)

Click on the _**Add New Menu Item**_ or _**New**_ button, as pointed out in the image. You will get the screen as shown in the image below:

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-create-new-menu-item-1.png)

Enter a name for the new menu item and click on the **Select** button to select the type of the menu item. 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-create-new-menu-item-2.png)

As shown in the image, click on the **Articles** and you will get a list down the option. From the new list, select **Category Blog**. Now, you will get a new option below the menu item type, named _**Choose a category**_. From that option, select **Product** as illustrated in the next image. 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-create-new-menu-item-3.png)

#### Edit SEBLOD Form Article Content Section <a id="edit-seblod-form-article-content-section"></a>

After you have finished, go to **Components -&gt; SEBLOD 3.x** and in the screen that is delivered, choose **Form & Content Type Manager**. It will give you the screen that is shown in the following image: 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-j2s-frontend-1.png)

As shown in the image, select the **Intro** tab. Select **All App Folders** and locate **J2Store\_Cart**. Add it by clicking on the **’&lt;’** symbol. Now, click on the _pencil_ symbol to edit the cart options, as shown in the image below: 

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-j2s-frontend-2-new.png)

You can edit the cart options by changing the text in the field as per your wish, for time being **mainimage\|cart**. Save the settings.

Now, go to the front end view of the site. You will get the home page as shown below: 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-cat-blog-view-1-new.png)

Your home page will display the products in your online store. Note that the new menu item, **Category Blog View** you have created is listed in the main menu list. Click on that and you will get the view as shown in the below image:

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-cat-blog-view-2-new.png)

### Single Article View <a id="single-article-view"></a>

To achieve the single article view, follow the steps, as illustrated in the images below:

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/single-article-view-1.png)

As shown in the image, click select the **Form & Content Types** menu. You will get the screen as shown below:

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/single-article-view-2.png)

Click on the **Article** and you will get the settings and configuration of **Article**. Check for the settings as shown in the next image.

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/single-article-view-3.png)

If the settings match the image above, you are done. If there is no _**J2Store\_Cart**_ listed on the left side, you can create on using the **+** sign on the right side. Now go to the frontend. All the articles will be listed in the site, as shown in the image below:

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/single-article-frontend-1.png)

You will get all the articles listed here. Click on any one article’s name, as shown underlined in the image. You will get the single article view.

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/single-article-frontend-2.png)

You can see the additional images, the cart, the **Next** button etc., in the view. If you hover on the additional images, they will be displayed in the main window, with a zoom effect.

This is how we achieve single article view.

### SEBLOD List & Search Type View <a id="seblod-list--search-type-view"></a>

In order to acieve the SEBLOD list and search view, you need to create a new menu item of type list and search. The following images illustrate the procedure.

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/list-view-backend-1.png)

As shown in the image, go to **Menus -&gt; Main Menu -&gt; Add New Menu Item**

You will get the screen to enter the menu items details. Enter a name for the menu item, say **SEBLOD List Articles** and then click on the _Select_ button to choose the menu item type. You will get a pop-up window as shown below:

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/list-view-backend-2.png)

Click on **SEBLOD** and you will get a list below. From the list, select **List & Search**. Now you will get a new field below the one you have dealt with just before, as **Search Type\(List\)**. Choose **Articles** in this field, as shown in the next image.

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/list-view-backend-3.png)

Leave other fields untouched. The Link will be created automatically. Now, **Save & Close** the menu item.

Go to frontend of your site.

You can see the menu item **SEBLOD List Articles**. Click on that and you will get the seblod articles listed down. These are depicted with the help of the following images.

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-list-frontend-1.png) ![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-list-frontend-2.png) ![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/seblod-list-frontend-3.png)

When you add the articles to your cart and click on the checkout link, the frontend of your site will look something like this:

![](https://raw.githubusercontent.com/j2store/doc-images/master/integrations/seblod/checkout-page.png)

You can checkout with a single click. It is not necessary for you to be a registered user. You can checkout as a guest. Later if you want, you can register.

#### Solve introtext displaying twice <a id="solve-introtext-displaying-twice"></a>

Sometimes you may face trouble in displaying short description and long description \(i.e.\) it displays the introtext twice instead of displaying the introtext and the fulltext.

If you face above issue, please try below solution which will solve your problem.

Copy /components/com_j2store/templates/default/view_ldesc.php

to

/templates/YOUR-TEMPLATE/html/com_j2store/templates/default/view_ldesc.php

Edit the file and replace the content with following code snippet

```text
 if($this->params->get('item_show_ldesc', 1)): ?>
	<div class="product-ldesc">
		 ?>
	
	 
	
	$fulltext = '';
	if ( $product->product_source_id > 0 ) {
		
		$db = JFactory::getDbo();
		$qry = $db->getQuery(true);
		$qry -> select('*') 
			 -> from('#__content')
			 -> where('id='.$product->product_source_id);
		$db->setQuery($qry);
		$item = $db->loadObject();
		$raw_text = '';
		$raw_text = $item->introtext;

		$st = strpos($raw_text,"::fulltext::") + 12 ;
		$len = strpos($raw_text,"::/fulltext::") - $st;
		$fulltext = substr($raw_text, $st, $len );
	}
	
		echo $fulltext;
 	?>

	div>
 endif; ?>
```

