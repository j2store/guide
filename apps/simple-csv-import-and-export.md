# Simple CSV import and export tool

## Important instructions before using this app <a id="important-instructions-before-using-this-app"></a>

1. Backup your site -Before you tend to use this app for import / export operations, you MUST be careful enough to take a full backup of your site. Use Akeeba backup to take the backup.
2. Export once -Export your products into .csv format once, to see how the format looks like. Check for field names. They should match.
3. Importing New Products -If you want to import new products, then you can ignore the product\_id field. And just make sure your products have a unique SKU. If an existing product has the same SKU as your new product, then the app will only update the existing product instead of creating a new one.
4. Unique SKU of the products MUST be unique. If there is a duplicate, it will result in an error.The app depends on SKU to find a product. So, if an SKU is found when searched, the existing product will be updated with the imported product details. If a match is not found, a new product will be created with the SKU.
5. Support for importing product options and / or product variants are not available.

## **Limitations**

Please note that the Simple CSV app does not support exporting of the Variable products, although you can import data like price after you created the variants manually

* It only supports Joomla articles as products. It DOES NOT support other catalog sources like K2, Zoo etc.
* Product options, categories cannot be imported.
* Support for importing product options and / or product variants are not available.
* It only supports the importing of the product data.

## Parameters <a id="parameters"></a>

1. Choose Import Type -You can choose to upload a CSV file or point the app to locate the file in a path. Recommended setting is: Upload.
2. Upload the CSV file -Click on the Browse button to select the CSV file for uploading.
3. Character Set -If you are not sure about the charter set of your file or do know what it is, then it is safe to leave it as Not Known. The app will attempt to determine the character set.
4. Update product if SKU already exists -If set to Yes, it will update existing products, if the SKU matches. Setting this to NO will only create new products.
5. Export Products -Clicking this button will export your products in csv format.

The following image illustrates the actions that are involved in import and export of .csv file.

![Simple CSV](https://raw.githubusercontent.com/j2store/doc-images/master/apps/simple-csv-import-export/csv-import-settings-edited.png)

A sample .csv file is given here for your testing purposes.

Below is a list of fields that are supported by the app for importing.

It is NOT necessary to have all these fields in your CSV. The following fields are the minimum required fields: sku, product\_type

* sku
* product\_id
* visibility
* product\_source
* product\_source\_id
* product\_type
* taxprofile\_id
* manufacturer\_id
* vendor\_id
* has\_options
* addtocart\_text
* enabled
* plugins
* params
* created\_on
* created\_by
* modified\_on
* modified\_by
* up\_sells
* cross\_sells
* main\_image
* thumb\_image
* additional\_images
* title
* alias
* introtext
* fulltext
* state
* catid
* created
* created\_by\_alias
* modified
* checked\_out
* checked\_out\_time
* publish\_up
* publish\_down
* version
* ordering
* metakey
* metadesc
* access
* hits
* metadata
* featured
* language
* xreference
* is\_master
* upc
* price
* shipping
* length
* width
* height
* length\_class\_id
* weight
* weight\_class\_id
* manage\_stock
* quantity\_restriction
* min\_out\_qty
* use\_store\_config\_min\_out\_qty
* min\_sale\_qty
* use\_store\_config\_min\_sale\_qty
* max\_sale\_qty
* use\_store\_config\_max\_sale\_qty
* notify\_qty
* use\_store\_config\_notify\_qty
* availability
* allow\_backorder
* isdefault\_variant
* quantity

**TIPS**

If you want to import more than one additional images \(in the additional\_images field\), you can use a pipe symbol \(\|\) to separate them.

**Example:** path/to/image1.jpg \| path/to/image2.jpg

