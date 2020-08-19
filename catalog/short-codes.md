# Short codes

Shortcodes are for Joomla article layouts.

The purpose of providing those short codes are because Joomla layouts are not under j2store’s control. It is developed and maintained by Joomla.

However product list layout / product pages are meant for displaying product and maintained by J2Store. It already has the code \(PHP code\) in its view files to display products and elements.

However, article layouts / core joomla layouts dont. That is why the short code is processed. So the short codes are provided for Joomla layouts. They wont work in J2Store’s product layouts.

```text
Adding more short codes to j2store pages (which already processes the products) would result in force processing / invoking j2store again and again resulting in performance issues.
```

## Additional short codes <a id="additional-short-codes"></a>

In addition to the primary short code, you can also use the following additional codes inside {j2store}{/j2store} . Each code should be separated by a pipe \(\|\) symbol.

To place this shortcode, first and most important thing is to change the Add to placement mode.

Go to J2Store &gt; Configuration &gt; Cart tabSet the Add to cart placement to Both or Within article using tag.Save.

### Example: <a id="example"></a>

{j2store}xx\|upsells\|crosssells{/j2store}

These additional short codes will work in all **Add to cart** placement modes. Please use these codes judiciously and wisely for better performance.

List of shortcodes available and their description

**cart** - Full cart with price, options and add to cart button{j2store}XX\|cart{/j2store}

 **Price** - This short code indicates both regular price and selling price{j2store}XX\|price{/j2store} ![Price shortcode](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/short-codes/shortcode_price.png)

![Add to cart shortcode](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/short-codes/shortcode_cart.png)

**Saleprice** - This code is for only the selling price{j2store}XX\|saleprice{/j2store}

![Sales price](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/short-codes/shortcode_sale_price.png)

**Regularprice** - This denotes only the regular price{j2store}XX\|regularprice{/j2store}

![Regular price](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/short-codes/shortcode_regular_price.png)

**Thumbnail** - This indicates a thumbnail is added via the j2store cart -&gt; images tab{j2store}XX\|thumbnail{/j2store} ![Thumbnail](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/short-codes/shortcode_thumb.png)

**Mainimage** - This shortcode indicates a main image is added via j2store cart -&gt; images tab{j2store}XX\|mainimage{/j2store}

![Main image](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/short-codes/shortcode_main.png)

**Mainadditional** - This is an indication of both main and additional images are added via j2store cart -&gt; images tab{j2store}XX\|mainadditional{/j2store}

![Main additional](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/short-codes/shortcode_mainadditional.png)

**Upsells** - This shows up-selling of products{j2store}XX\|upsells{/j2store}

![Upsells](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/short-codes/shortcode_upsells.png)

**Crosssells** - This shows cross selling of products{j2store}XX\|crosssells{/j2store} ![Crosssells](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/short-codes/shortcode_crosssells.png)

### Example <a id="example-1"></a>

{j2store}1\|thumbnail\|cart{/j2store}

![Cart thumb](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/short-codes/shortcode_cart_thumb.png)

### Video Tutorial: <a id="video-tutorial"></a>

{% embed url="https://youtu.be/YwgwQj83cMo" %}





