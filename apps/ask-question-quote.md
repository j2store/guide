# Ask question / quote

This app allows customer to enquire a product or to ask quote for a product through mail.

Using this app itself you can use your store as catalog mode since this app has an option to hide the add to cart button. Clicking on single button will enable the communication between store owner and customer.

**Requirements**

* PHP 5.4 or higher
* Joomla 3.3 or above
* J2Store 3.2.x or above

**Switch off catalog mode:**

**NOTE:** **If you are having the shop in catalog mode, the ask quote button wouldn’t come up on the storefront.**

Alternatively, you could turn off the catalog mode and hide the add to cart buttons in the site using the **Hide add to cart button for all products?** in the basic settings of the Ask quote plugin.

**Installation**

1. Use the Joomla installer to install the app.
2. In the backend, go to J2Store Dashboard -> Apps as shown in the image below.
3. Click Enable in the Ask question / quote app.

![Ask quote](https://raw.githubusercontent.com/j2store/doc-images/master/apps/ask-quote/ask-quote-dashboard.png)

4\. Once the app is enabled, open the app to configure the settings.

**Global level:**

In the global settings of the app, you can configure&#x20;

* How and where the ask quote app would appear at the storefront.
* The look of the email that is triggered when a user submits the ask quote form.
* The layout of the ask quote modal form.

#### **Basic Settings**

* **Enable Ask quote button for all products**

Select YES or NO to enable and disable the Ask quote button for all products.

* **Hide add to cart button for all products**

Select YES or NO to hide the Add to cart button.

* **Hide Zero Price Cart Button**

Select yes or no to hide the cart if the the price of the product in the cart is zero

* **Display form style**

Select the view of the Ask Quote form.

POP-UP: Select this to display the ask quote form in a separate pop-up window.

Accordion: Select this to display the ask quote form in an accordian view

* **Display position**&#x20;

Choose whether you wish to have the add to quote form before or after the cart.

* **Display button / link in**

Select the location (Product view, category view, Both views) where the Ask Quote button should be displayed.

* **Display button/link**

Selecting display type here will make the text to be displayed in button / link.

![Ask quote settings](https://raw.githubusercontent.com/j2store/doc-images/master/apps/ask-quote/ask-quote-settings.png)

* **Display text for button/link**

Change the button text / link text by entering custom text here.

Use the language constant PLG\_J2STORE\_PRODUCTQUOTE\_LINK\_TEXT to translate the text when you are using multilingual site.

#### Email Configuration

&#x20;**Include label for custom fields:**&#x20;

If you wish that the label of the custom fields you use should be available on the email, then set this to Yes.

**Mail sent to:**

You could choose whether the user alone or admin alone or both should receive the ask quote email.

**Email body:**

Enter the body of the email here. You can use the below shortcodes in the text editor:

\[SITENAME]\
&#x20;\[FIRST\_NAME]\
&#x20;\[LAST\_NAME]\
&#x20;\[PHONE\_1]\
&#x20;\[PHONE\_2]\
&#x20;\[EMAIL]\
&#x20;\[COMPANY]\
&#x20;\[TAX\_NUMBER]\
&#x20;\[ADDRESS\_1]\
&#x20;\[ADDRESS\_2]\
&#x20;\[CITY]\
&#x20;\[ZIP]\
&#x20;\[COUNTRY\_NAME]\
&#x20;\[ZONE\_NAME]\
&#x20;\[PRODUCT\_NAME]\
&#x20;\[PRODUCT\_SKU]\
&#x20;\[PRODUCT\_PRICE]\


**To Display the custom field data**

To display the custom field information entered by the user when filling form in an email the customer and admin receive, it is possible by adding the shortcode of respective custom field in the Email body editor.&#x20;

For example, if you are having text area as a custom field in your product quote form, then copy the field name(you can get it in custom field section J2Store > Setup > Custom fields) and paste it in Email body editor. The custom field shortcode should be enclosed with square braces. For example, \[message].

&#x20;Refer the image below,

![](../.gitbook/assets/screenshot-localhost-2020.08.14-17\_37\_38.png)

**Email subject**

Choose a subject line for the quote email notifications.

With that, the Email configuration is complete.

**Layout**

If you would like to add / remove the fields in product quote form without affecting checkout form fields, it is possible in this section.

In this section, you can create the custom form by adding field shortcode given in the top of the layout tab page and display that field in the form.

To add any new fields, go to J2Store > Setup > Custom fields. Click NEW to create new field.

Here is how you could create a new custom field.

Now, in form layout add the shortcodes of fields you want to display in product quote form.

To add the custom field shortcode, copy the field name in J2Store > Setup > Custom fields section and paste it in the form. The field name should be enclosed with square braces. For example, \[message].

&#x20;&#x20;

![Ask quote custom field](https://raw.githubusercontent.com/j2store/doc-images/master/apps/ask-quote/ask-quote-custom-field.png)

![Ask quote custom field list](https://raw.githubusercontent.com/j2store/doc-images/master/apps/ask-quote/ask-quote-cust-fiel-list.png)

![Layout of the fields](https://raw.githubusercontent.com/j2store/doc-images/master/apps/ask-quote/ask-quote-layout.png)

That's it! The data entered on this custom field at the ask quote form during quote submission would show up at the ask quote email.

#### **Enable quote for per product**

1. This app allows you to enable Ask quote button for specific product.
2. Go to Article manager and open the article.
3. Under the J2Store cart tab, navigate to the Apps menu.
4. Enable the Ask quote button by setting YES to Enable ask question / quote. Refer the image below.

**Frontend**

**Ask quote enabled on a single product- At the product article**

&#x20;&#x20;

![Ask quote frontend](https://raw.githubusercontent.com/j2store/doc-images/master/apps/ask-quote/ask-quote-frontend.png)

#### Ask quote enabled on All products- on the global settings

![Ask quote enabled on all products](https://raw.githubusercontent.com/j2store/doc-images/master/apps/ask-quote/ask-quote-all-pro-front.png)



**Support**

Still have questions? Reach out to us via the Priority ticket system or the Support Request form.
