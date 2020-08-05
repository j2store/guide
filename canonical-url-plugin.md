# Canonical URL Plugin

This plugin solves the duplicate URL problem in search engines by adding appropriate Canonical tags for J2Store products and Articles.

## Introduction <a id="introduction"></a>

Let us suppose that we have three products based on tags T shirts, Summer and Winter collection. So a product say Printed Tee falls under all the above three categories.

This being the case, we create 3 tags, namely T shirts, Winter and Casual collection. All the three tags are being associated with the product Printed Tee. Now, this might create multiple URLs which when indexed by Search engines might create duplications.

So to avoid this, the canonical URL plugin is used. When the canonical plugin is enabled and the layout is Tag view layout, the canonical menu chosen in the menu settings would be given higher priority when compared to the one set on the product level.

Now that we know the purpose of the plugin, let us see how it has to be configured.

## Configuration <a id="configuration"></a>

The plugin doesn’t have much of options to be configured at the plugin level. The plugin could be found under Extensions-&gt;Plugins. It would be named as **System - J2Store Canonical.**

The setting found in the plugin would allow you to choose the canonical tag. There are two options available: \*\*1.\)Menu canonical tag 2.\)Current URL \*\*

![Introduction](https://raw.githubusercontent.com/j2store/doc-images/master/canonical-url-plugin/options%20in%20settings.png)

When the menu canonical tag option is chosen, the tag that is associated on the Item view canonical tab would be taken into account and the URL for the tag associated with the canonical menu option in the menu settings would be displayed as the URL while indexing happens.

Let us consider that Summer is the tag associated with the canonical menu option in the menu settings, then the indexing would have the URL associated with that tag.

![indexing](https://raw.githubusercontent.com/j2store/doc-images/master/canonical-url-plugin/screenshot-localhost-2018-07-25-18-09-34.png)

The canonical URLs would **NOT** be visible for naked human eye. They would only be available on the meta tags of the head section of the page and would be used while indexing happens. The URL found in the frontend meta tag would be as follows:

![Frontend meta](https://raw.githubusercontent.com/j2store/doc-images/master/canonical-url-plugin/Selection_078.png)

When there are no tags associated to the canonical menu option in the Item view canonical tab of the tag view menu, and there is a main tag set on the product, and the canonical type option in the plugin setting is set to Menu canonical tag, then the main tag would be associated with the index URL.

![No tags](https://raw.githubusercontent.com/j2store/doc-images/master/canonical-url-plugin/screenshot-localhost-2018-07-25-17-50-17.png)

The main tag chosen in the product article is as follows:

![](https://raw.githubusercontent.com/j2store/doc-images/master/canonical-url-plugin/screenshot-localhost-2018-07-25-18-27-58.png)

Now the tag displayed on the meta tag of the frontend would be as follows: ![meta tag](https://raw.githubusercontent.com/j2store/doc-images/master/canonical-url-plugin/Selection_079.png)

When the canonical type is chosen as Current URL on the plugin parameters, a validation would be done if there are any tags associated on the menu parameters. If so, then the tag associated with the menu parameter would take effect. If not, then a check would be done if there is any main tag associated on the product, and if not, the current URL itself would be used.

Thus the canonical plugin helps in eliminating duplicate URL issues while indexing is done by search engines.

