# Creating an integration plugin for your component

This topic is split into the following sections to make it easier for you to understand:

* Introduction
* The concept
* Integrating with your component
* Get the product form fields
* Save product data
* Supply item data to J2Store Display the cart

## Introduction <a id="introduction"></a>

Integrating J2Store with your extension is pretty straightforward. Since Version 3, we implement a flexible Plugin API and the entire J2Store core is re-written from scratch using the Framework on Framework \(FOF\).

So all you have to do is create an integration plugin for your component \(using your component’s events\). It can be a system plugin or a plugin specific to your component.

## The Concept <a id="the-concept"></a>

J2Store can treat any item \(an article, an event, a photo\) as a product. All it needs is the name of the source \(read as your component’s name. Example: com\_foo\) and the source item’s ID.You can use your component’s plugin events to display the J2Store’s Product Form, Save it and then Render it \(in the front end\)So basically three events are sufficient to integrate J2Store in your component.

Let me give you an example of how J2Store is integrated with the Joomla articles

1. **onContentPrepareForm**

Here we inject the J2Store’s Product Form into the Article’s Edit view. So the store owner treats the article as product and fills in the form.

1. **onContentAfterSave**Here, we catch the data of the filled-in product form and save it to the J2Store’s tables. While saving, we save two important variables
2. **product\_source** = The name of the component which serves as the catalog source. In this case, com\_content
3. **product**_**source**_**id** = The id of the item that is treated as a product. In this case, the article id.
4. **onContentAfterDisplay** So, we have displayed the form, saved the data. Now it is time to inject the cart block \(price, quantity field, Add to cart button\) into the article.This method takes care of it.

## Integrating with your component <a id="integrating-with-your-component"></a>

Let us integrate J2Store with your component

NOTE: This guide assumes that you have a good understanding of Joomla Plugins and Events

Start the integration by creating a system plugin or plugin specific to your component. The plugin should have four events for

1. Display the product form fields in your item
2. Save the product data \(after your item data is saved\)
3. Supply data to j2Store \(via a J2Store event\)
4. Display the cart

**Display the product form fields**

The first and foremost task is to get the J2Store’s Product form fields to display inside your component’s item.

If your component fire’s an event after displaying the form, then the task is pretty easy. You can create a system plugin with the event and call the following lines

```text
  ```$app = JFactory::getApplication();
     //the id of your item. This will be treated as the product_source_id
  	 	$id = $app->input->getInt('cid');

  	 	$productTable = F0FTable::getAnInstance('Product' ,'J2StoreTable');
  			
  	$productTable->load(array('product_source'=>'com_foo', 'product_source_id' =>$id));
  	
  		$product_id = (isset($productTable->j2store_product_id)) ? $productTable->j2store_product_id : '';

  	 	$inputvars = array(
  	 			'task' =>'edit',
  	 			'render_toolbar'        => '0',
  	 			'product_source_id'=>$id,
  	 			'id' =>$product_id,
  	 			'product_source'=>'com_foo',
  	 			'form_prefix'=>''
  	 	);
  	 	$input = new F0FInput($inputvars);

  	 	@ob_start();
  		F0FDispatcher::getTmpInstance('com_j2store', 'product', array('layout'=>'form', 'tmpl'=>'component', 'input' => $input))->dispatch();
  		$html = ob_get_contents();
  		ob_end_clean();
  		return $html;```
```

**Save the product data**

Saving the data is also very simple. Just capture the filled-in form data \(Usually in your After Save event\)Then just pass the data \(can be either an array or an object\) to

```text
```F0FModel::getTmpInstance('Products', 'J2StoreModel')->save($data);```
```

IMPORTANT: The array or object should have the product_source and product_source\_id . Otherwise, J2Store will not be able to process your item as product.

Example:

```text
product_source='com_foo'
product_source_id=$id //the ID of your item
```

**Supply product data**

You will have to supply a few important information to J2Store. Example, the product name, its url etc. J2Store has an event called: **onJ2StoreAfterGetProduct\(&$product\)** NOTE: If your Integration plugin is specific to your component, then you should create a system plugin with this event. Refer the K2 integration plugin for example.

```text
function onJ2StoreAfterGetProduct(&$product) {	if(isset($product->product_source) && $product->product_source == 'com_foo' ) {		//assign		$product->product_name = $name;	
```

//supply a url to edit the item. This is essential. Because j2store will use this to link

**Display the cart block**

Time to get the add to cart block for your item.Here are the three lines that will get you the entire cart block.

```text
$html = '';
$product = F0FTable::getAnInstance ( 'Product', 'J2StoreTable' )->getClone ();
if ($product->get_product_by_source ( 'com_foo', $id )) {
		$html = $product->get_product_html();
	}
	echo $html;
```

You have a number of methods in the product object.

To get the main image

$product-&gt;get_product_images\_html\(‘main’\);

To get cross sell products

$product-&gt;get_product_cross_sells_html\(\);

To get up sell products

$product-&gt;get_product_upsells\_html\(\);

Refer the the content plugin of J2Store for more detailed information and methods of implementing.\(plugins/content/j2store/j2store.php\)

