# Moving the description

## To move the description below the price section of the product <a id="to-move-the-description-below-the-price-section-of-the-product"></a>

When you try to move the description below the price section, for a simple product, an override has to be carried out as follows:

* Copy the file “view\__simple.php” from the path “components/com\__j2store/templates/your site’s sub-template/“.
* Navigate to “/templates/your site’s template/html/com\__j2store/templates/your site’s sub-template/” and paste the file “view\__simple.php”.
* Around line 29, you would find the following line:

```text
<?php echo $this->loadTemplate('price'); ?>
```

* **Change it to:**

```text
<?php echo $this->loadTemplate('price'); ?>
<?php echo $this->loadTemplate('sdesc'); ?>
<?php echo $this->loadTemplate('ldesc'); ?>
```

If you wish to remove the description that is displayed at the bottom of the images, navigate to line 64, you would find this:

```text
<?php if($this->params->get('item_use_tabs', 1)): ?>
		<?php echo $this->loadTemplate('tabs'); ?>
	<?php else: ?>
		<?php echo $this->loadTemplate('notabs'); ?>
	<?php endif; ?>	
```

* **Change it to:**

```text
<?php if($this->params->get('item_use_tabs', 1)): ?>
		<?php //echo $this->loadTemplate('tabs'); ?>
	<?php else: ?>
		<?php //echo $this->loadTemplate('notabs'); ?>
	<?php endif; ?>	
```

This would display the description \(both short and long\) below the price info. And remove the description section below the images.

The above steps have to be carried out for other product types as well. The override specified here would take effect on the item view page of a simple product. The files to be overridden are “view\__variable.php”, “view\__configurable.php” and “view\_downloadable.php”

## To move the description above the price section of the product <a id="to-move-the-description-above-the-price-section-of-the-product"></a>

When you try to move the description above the price section, for a simple product, an override has to be carried out as follows:

* Copy the file “view\__simple.php” from the path “components/com\__j2store/templates/your site’s sub-template/“.
* Navigate to “/templates/your site’s template/html/com\__j2store/templates/your site’s sub-template/” and paste the file “view\__simple.php”.
* Around line 29, you would find the following line:

```text
<?php echo $this->loadTemplate('price'); ?>
```

* **Change it to:**

```text
<?php echo $this->loadTemplate('sdesc'); ?>
<?php echo $this->loadTemplate('ldesc'); ?>
<?php echo $this->loadTemplate('price'); ?>
```

If you wish to remove the description that is displayed at the bottom of the images, navigate to line 64, you would find this:

```text
	<?php if($this->params->get('item_use_tabs', 1)): ?>
		<?php echo $this->loadTemplate('tabs'); ?>
	<?php else: ?>
		<?php echo $this->loadTemplate('notabs'); ?>
	<?php endif; ?>	
```

* **Change it to:**

```text
	<?php if($this->params->get('item_use_tabs', 1)): ?>
		<?php //echo $this->loadTemplate('tabs'); ?>
	<?php else: ?>
		<?php //echo $this->loadTemplate('notabs'); ?>
	<?php endif; ?>	
```

This would display the description \(both short and long\) above the price info. And remove the description section below the images.

The above steps have to be carried out for other product types as well. The override specified here would take effect on the item view page of a simple product. The files to be overridden are “view\__variable.php”, “view\__configurable.php” and “view\_downloadable.php”

