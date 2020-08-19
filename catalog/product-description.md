# Product description

By default the joomla article considers the text as short description. When you use page break or read more, you will see red or grey line in article.

Under that whatever text has entered that considered as Long Description.

![Article readmore](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/product-description/article_readmore.png)

![Short long description](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/product-description/short_long_description.png)

## According to J2store <a id="according-to-j2store"></a>

J2Store takes the introtext column as the short description and fulltext column as the long description.

These two columns are in the joomla’s \_content \(article table\)

The Article manager divides the text \(content\) into two and saves it based on the readmore break.

In J2store, you can enable and disable the display of short description and long description in both category view and product view.

### In version 2 <a id="in-version-2"></a>

Sometimes “short description” is enabled in the setting with “long description” disabled but the list layout shows both text plus read-more text.

The above issue seems to be occuring while triggering the content plugins.

Old content plugins process the $item-text as $item-&gt;introtext

So, the following line \(line number 576\) that is added for old plugin compatibility, might be causing the issue

It assigns the whole text as introtext// Old plugins: Use processed text as introtext$item-&gt;introtext = $item-&gt;text;

### In version 3 <a id="in-version-3"></a>

The read more break works fine.

### Support <a id="support"></a>

Still have questions? You can post in our support forum: [Click here](http://j2store.org/forum/index.html)

