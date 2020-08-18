# Cart not Working

This is one among the most commonly reported issues. There might be a number of reasons why this happens and here are some of the prominent reasons. The following article might be of help to you in troubleshooting cart-related issues.

## Issue: <a id="issue"></a>

Item is added to cart. Clicking on the inline link doesn’t take you to the cart page.

## Causes & Resolutions: <a id="causes--resolutions"></a>

Check if a menu has been created of the type J2Store-&gt;Cart and access has been set as anything apart from Public.

**Screenshot:**

![cart menu](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/cart-not-working/cart-menu.png)

### Product type: <a id="product-type"></a>

Check your product type. If you have a booking type product, then make sure that the cache expiration time is set to minutes higher than 0 in the booking app’s settings.

![Product type](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/cart-not-working/image.png)

 Ensure that the time zone is set to the corresponding time zone as per the store profile. For example, if you have set up Denver, USA as the store address, then the corresponding time zone should be chosen in your Joomla configuration \(under System-&gt;Global configuration-&gt;Server tab-&gt;Denver\).

![configuration](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/cart-not-working/config.png)

![Image2](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/cart-not-working/image%20%282%29.png)

### Plugins: <a id="plugins"></a>

 Check if the EU-privacy directive plugin is enabled under Extensions-&gt;Plugins. If so, disable this plugin and that should solve the issue.

### Caching: <a id="caching"></a>

 Check for cache plugins like JSGcache, Shlib, Litespeed cache, system-page cache, system-J2page cache. Check if caching is enabled in Joomla global configuration, check if varnish caching and server-side caching is enabled. If so, disable them and then check.

## Checking if the site has got cache: <a id="checking-if-the-site-has-got-cache"></a>

To check if the issue is because of caching, follow the below steps:

* Visit the cart page.\(If you have enabled caching on your site, then the cart page would be cached by now\)
* Go back to the products page and add products to the cart page.
* Visit the Cart page again. It shows no items from cart \(because this page is a photocopy from the caching plugin, say for example Litespeed cache\)
* Use the non-sef URL of the cart page \(Same page, same logic… just the url is different\)

Non-sef URL format: [https://yoursite.com/index.php?option=com\_j2store&view=carts](https://yoursite.com/index.php?option=com_j2store&view=carts)

In our case, LiteSpeed being the caching component used on our site, It looks up for this URL in its cache. None found. So it allows the request to reach the webserver, which then renders the page with its dynamic content.

Cart contents show up.

**Solution:**

Ask your hosting service provider to remove LiteSpeed or exclude the dynamic pages like cart and checkout.  


