# Advanced variable

This app extends the variable product type. With this app you can treat the options as variants and can maintain the stock level.

**Requirements**

* PHP 5.4 or higher
* Joomla 3.x or higher
* J2Store 3.2.15 or higher

**Installation**

* Download the package from our site and install it in your site using Joomla Installer.
* After installing the app, in the Joomla backend go to J2Store &gt; Dashboard &gt; Apps and enable it.
* There is no major settings to be configured inside the app. Go to article manager and create new article with product type Advanced Variable.

**Advanced Variable Product**

**STEP-1**

* Go to article manager &gt; Create a new article
* Move to J2Store cart tab
* Choose Treat as a Product YES
* Choose product type Advanced variable
* Click Save and Proceed.

 

![Advanced variable](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_product.png)

![Save and proceed](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_product-_save.png)



**STEP-2**

* 2.1 Navigate to the General tab
* Set YES to visible in storefront
* 2.2 Navigate to Images tab
* Add Thumbnail image, Main image and Additional image.

**STEP-3:**

* Navigate to Variants tab and type the first few letters of the unique name of the product options in the search box.
* Choose the option from the dropdown and click save.
* Set the values for option and then save again.

![Adding variants](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_variants.png)

   

![Adding options](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_var_add_opti.png)

![Setting option values](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_set_opt_val.png)

![Adding values to option and setting price](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_add_opt_price.png)

![Adding option values and saving](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_save_opt_prices.png)



Its no matter you are using options as variants or not. Whatever it is you must generate the varaints once. Otherwise the error will be notified.

**How to use options as variants?**

On saving the article, you will be having checkbox at the **Use as variant** column. Check this checkbox to use the options you added as variants.

![Setting options as variants](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_set_as_vari.png)

Before generating variants, check the checkbox next to the Required column and click save. Once saved, click **Generate Variants** button.

 

![Generating variants](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_gen_variants.png)

After generating variants, click **Open all** button to set all the product requirements such as price, shipping dimensions, stock and press save button.

 

![Open all variants](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_openall.png)

![Variants list](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_var_list.png)



Now check the product in frontend.

 

![Frontend view](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_frontend.png)

When using options as variants, at frontend you could see the option with price prefix. This should not be shown when displaying options as variants. To avoid this, you just open the option value and save once. Please refer the image below,  

![Setting option values](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_set_option_values.png)

![Save changes](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_save_changes.png)

Now check the product in frontend ![Frontend view](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_front.png) 

**Using as Options**

If you would like not to use options as variants, do the instructions given below,

* Go to article manager and move to J2Store cart tab.
* Navigate to Variants tab
* Uncheck the Use as variants checkbox \(Don’t delete the varaints\) and click save.
* After saving, move to variants tab and click on Set option values to set the price prefix for option values. Refer the image below,

 

![Unchecking the variant checkbox](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_uncheck_vari_checkbox.png)

![Setting option values](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_setting_opt_val.png)



Now check the product in frontend

 

![Frontend view](https://raw.githubusercontent.com/j2store/doc-images/master/apps/advanced-variable/adv_variable_frontview.png)

This is how an advanced variable can be used.

