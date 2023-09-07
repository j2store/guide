# To Display Both the main Image and the additional image in the product view page

Please carry out the override as follows:

Navigate to “/components/com_j2store/templates/default/view_images.php”.

Copy the above file and paste it under “/templates/your template/html/com\_j2store/your sub-template”.

Now edit the file under the overridden path and around line 39, you would find this:



````
<?php echo J2Store::product()->displayImage($this->product,array('type'=>'ViewMain','params' => $this->params)); ?>
<?php endif; ?>
</div>
<?php endif; ?>```
````

&#x20;`Change it to:`&#x20;



````
```    <?php elseif(!empty($this->product->main_image)):?>
    <?php echo J2Store::product()->displayImage($this->product,array('type'=>'ViewMain','params' => $this->params)); ?>
    <?php endif; ?>
    </div>
    <?php endif; ?>
    <div class="j2store-thumbnail-image">
    <?php if(JFile::exists(JPATH_SITE.'/'.JPath::clean($this->product->thumb_image))):?>
        <img itemprop="image" alt="<?php echo (!isset($this->product->thumb_image_alt) || empty($this->product->thumb_image_alt)) ? $this->product->product_name:$this->product->thumb_image_alt ;?>" title="<?php echo $this->product->product_name ;?>" class="j2store-img-responsive j2store-product-thumb-image-<?php echo $this->product->j2store_product_id; ?>" src="<?php echo $image_path.$this->product->thumb_image;?>" />

    <?php elseif(!empty($this->product->thumb_image)):?>
    <?php echo J2Store::product()->displayImage($this->product,array('type'=>'Thumb','params' => $this->params)); ?>
    <?php endif; ?>
    </div>          
````

Save.

Now the main image as well as the thumbnail image should appear on the product view page.
