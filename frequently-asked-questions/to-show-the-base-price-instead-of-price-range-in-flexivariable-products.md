# To show the base price instead of price range in flexivariable products

If you don’t like the price range of the variants getting displayed on the storefront, then you could replace it with the default base price.

Following are the steps to be followed:

## Steps: <a id="steps"></a>

* Navigate to the Flexi variable product.
* Set the default variant by clicking on the star next to the variant. ![Setting default variant](https://raw.githubusercontent.com/j2store/doc-images/master/frequently-asked-questions/hiding-price-range-in-flexivar/freq-as-que-flexivar-default-variant.png)
* Navigate to the menu manager-&gt;choose the menu of the flexi variable product.
* In the item view options in category listings and Item view options tab, set the option

## Regular Price to Show and base price to show. <a id="regular-price-to-show-and-base-price-to-show"></a>

![Menu settings](https://raw.githubusercontent.com/j2store/doc-images/master/frequently-asked-questions/hiding-price-range-in-flexivar/freq-as-que-flexivar-base-price.png)

* Navigate to /templates/your template/html/com\_j2store/templates/ [sub-template](http://docs.j2store.org/catalog/where-can-i-find-my-sub-template)
* Create a file called “default\_flexiprice.php” and paste the code in the following gist:



```text
 https://gist.github.com/sowbagyalakshmi/451d33fce24cf111b29e06e23b6be6d1
```

* At the same path, create another file called view\_flexiprice.php and paste the code in the following gist:

```text
https://gist.github.com/sowbagyalakshmi/d1a1749bf17c45c0ca251bde4ba60ed3
```

Now the base price would be displayed instead of the price range.

![Item view ](https://raw.githubusercontent.com/j2store/doc-images/master/frequently-asked-questions/hiding-price-range-in-flexivar/freq-as-que-flexivar-item-view.png)

![List view showing base price](https://raw.githubusercontent.com/j2store/doc-images/master/frequently-asked-questions/hiding-price-range-in-flexivar/freq-as-que-flexivar-list-view.png)

