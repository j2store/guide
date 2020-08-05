# To display the UPCE/BAN/ISBN on the product page

Navigate to **“/templates/your template/html/com\_j2store/templates/your site’s sub-template/“,** create a file called ”**default\_sku.php**” and paste the following content there:



```text
<?php
/**
* @package J2Store
* @copyright Copyright (c)2014-17 Ramesh Elamathi / J2Store.org
* @license GNU GPL v3 or later
*/

// No direct access
defined('_JEXEC') or die;
?>

<?php if(!empty($this->product->variant->sku)) : ?>
<div class="product-sku">
<span class="sku-text"><?php echo JText::_('J2STORE_SKU')?>
</span>
<span itemprop="sku" class="sku">
<?php echo $this->product->variant->sku; ?>
</span>
<br>
<span itemprop="upc" class="upc>
<?php echo $this->product->variant->upc; ?>
</span>
</div>
<?php endif; ?>
```

Create another file called ”**view\_sku.php**” and paste the following content there:  


```text
<?php
/**
* @package J2Store
* @copyright Copyright (c)2014-17 Ramesh Elamathi / J2Store.org
* @license GNU GPL v3 or later
*/

// No direct access
defined('_JEXEC') or die;
?>
<?php if($this->params->get('item_show_product_sku', 1) && !empty($this->product->variant->sku)) : ?>
    <div class="product-sku">
        <span class="sku-text"><?php echo JText::_('J2STORE_SKU')?> :</span>
        <span itemprop="sku" class="sku"> <?php echo $this->product->variant->sku; ?> </span>
        <br>
        <span itemprop="upc" class="upc"> <?php echo $this->product->variant->upc; ?> </span>
    </div>
<?php endif; ?>
```

This would display the EBAN in the list view and item view pages.

