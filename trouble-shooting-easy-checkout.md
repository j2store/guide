# Trouble shooting issues

J2Store and Easy checkout shares most of the language strings.

For example, if your site is in Dutch language Here are the steps to create dutch translation file for easy checkout.

Copy /administrator/language/en-GB/en-GB.com\_easycheckout.ini

To /administrator/language/nl-NL/en-GB.com\_easycheckout.ini

Now rename the file **en-GB.com\_easycheckout.ini** under /administrator/language/nl-NL/ to

**nl-NL.com\_easycheckout.ini**

Now edit /administrator/language/nl-NL/nl-NL.com\_easycheckout.ini

Now replace the values for all the language strings related to easy checkout.

For example,EASYCHECKOUT_CUSTOMER_INFORMATION=“Customer information”

Replace Customer information with your value and save.

**How to reorder checkout fields ?**

As like J2Store’s standard checkout, the checkout fields could also be re-ordered in Easy checkout as well. You could place the checkout fields wherever you wants inside the checkout page.

Here are the steps to be followed:

Go to J2Store &gt; Configuration &gt; Checkout layout tab

![](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-01.png)

You will see the textarea for 3 layout sections \(Billing, Shipping, Payment\), where you could add the shortcode of the checkout fields.For example, \[first\_name\]

The checkout page will display all the fields that are added here.

To add all the checkout core fields, click on Pre-populate / Restore fields at the right corner of the page.

Now the page will be looking like below:

  

![](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-02.png)

Now re-order the fields as your wish. See the screenshot below: 

![](https://raw.githubusercontent.com/j2store/doc-images/master/easy-checkout/easy-checkout/easycheckout-03.png)

If you have created custom fields and wants to add reorder them, that could also be possible.For example, if you have field Delivery date, then add the shortcode \(\[deliverydate\]\) of it inside the text area. **How to create template override for Easy checkout ?**

If you would like to customize the Easy checkout page, that could be possible by creating template override. Carrying out customizations through template override will not overwrite the changes if you update it in future.

Here are the instructions to be followed:

The files that controls Easy checkout page are located at

/components/com\_easycheckout/views/checkout/

For example, if you wants to customize the login form, then copy below file

/components/com_easycheckout/views/checkout/tmpl/default_login\_form.php

And paste it under

/templates/YOUR-SITE-TEMPLATE/html/com_easycheckout/checkout/default_login\_form.php

Edit

/templates/YOUR-SITE-TEMPLATE/html/com_easycheckout/checkout/default_login\_form.php

Make your changes and save.

