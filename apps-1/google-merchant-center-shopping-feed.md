# Google merchant center shopping feed

The app helps you export products for Google Shopping feed.New to the term Google Merchant? More details can be found at [Google Merchant Center](https://www.google.com/retail/solutions/merchant-center/#?modal_active=none)

If you have any doubts or queries regarding Merchant center service, visit [Google merchant Support center](https://support.google.com/merchants/#topic=7259123)

Parameters

1. Google Category - Google has its own detailed taxonomy \(or\) classification of products. Input the category to which all your products belong to. For list of categories provided by Google, refer this [link.](https://support.google.com/merchants/answer/6324436?visit_id=636970474443851376-580915083&rd=1)
2. CSV file Name -Name of CSV file used to upload in merchant center. Make sure the file name does not contain any spaces \(use underscores or hyphen symbol instead of space\).
3. Product Condition -Please select your product condition from this list. There are three options \(New, used, refurbished\)

![gmcsf01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/google-merchant-center-shopping-feed/gmcsf01.png)

**Configure Fields**

* There are a list of fields to be uploaded to google merchant center feed.
* You may enable or disable the fields in this section.
* The fields in Enabled state are considered during Feed generation.
* Please refer Google’s Documentation for List of Fields used for the Google Shopping Feed and their detailed specifications.

![gmcsf02](https://raw.githubusercontent.com/j2store/doc-images/master/apps/google-merchant-center-shopping-feed/gmcsf02.png)

Below is a list of fields that are supported by the app.

```text
Field name                      Description

id                              Product id
title                           Product name
description                     Product Short Description
google_product_category         Value given in the parameters
product_type                    Product's Category
link                            Link to the Single Product view
mobile_link                     Link to the Single Product view
image_link                      Link of the main image.
additional_image_link           Link of the thumbnail image.
condition                       As per settings in above parameter. availability calculated based on product's stock               
price                           Price of the product
sale_price                      Price of the Product
gtin                            custom field
mpn                             sku (product sku is supplied)
brand                           Manufacturer
identifier_exists               Calculated based on Google's constrains (takes two values TRUE or FALSE)
```

**Generate Feed and upload to Merchant center**

Click on the **Download Feed** button to download the feed. Verify the fields and upload the feed to the merchant center for publishing your products to Google Shopping service.

More details on configuring your merchant account and uploading shopping feed can be found at [Google merchant Support center](https://support.google.com/merchants/#topic=7259123)

