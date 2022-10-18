# Currency

J2Store allows you to sell in multiple currencies. You can create as many currencies as you like.You can either set the exchange value of the currency manually or allow J2Store to fetch in real-time from the Google Financial API. (In Store configuration, you should set the Auto update currency to YES)

**Creating a new currency**

Click the New button to start the currency creation process.

* **Currency Title**

Title is very important and it should be given in a proper way. E.g., US Dollars.

* **Currency Code**

The currency code must be selected from the list given. A new code of users choice cannot be added to the list. E.g. USD

* **Currency Symbol**

This is a single figure which is used globally for referring the currency. For e.g., the United States Dollar is denoted by the symbol $. This symbol is used by many countries for their currencies, though, this represents US Dollars by default.

* **Symbol Position**

The symbol is placed on anyone side of the currency name, according to the standards of the country that currency belongs to. For e.g., the $ is always prefixed (before currency name) like this: $ 500.00 and some currencies may also be suffixed (after currency name), tentatively like this: 500.00 $.

* **Decimal Places**

This indicates the number of decimal places after the ’.’ in the currency value. Usually, decimal places are 2.

* **Decimal Separator**

By default, a period or dot(.), serves the purpose of a decimal separator across the globe. Some countries may also use comma(,) as separator. In any of the case, based on the separator only, the price entered in product page will be processed for checkout and payment procedures.

* **Thousands Separator**

A comma is the thousands separator worldwide. This separator is also referred for payment process.

* **Value**

This option is used to set the default currency. If the value is set be 1.000000 for a particular currency, it will serve as the default currency. All other currencies will be in relation with this. For e.g., if US $ is been set the value 1, it will be the default currency and the corresponding value will be 0.81 for Euro. In this way J2Store will calculate the prices for products based on currency transitions.

* **Status**

This option sets the status of publication of the currency. If it is set to be Published, then it will be available for payment process. Otherwise, it will not be available for payments.

![Adding a new currency](https://raw.githubusercontent.com/j2store/doc-images/master/set-up/currency/Currency\_Add.png)

The image above indicates how to add or edit a currency.

**Display the prices with comma**

Prices should also be entered with the . (DOT) as the decimal separator. In the currency settings screen, as mentioned in the below picture, you can change the formatting option. This will automatically display the prices with comma. ![Displaying prices with comma](https://raw.githubusercontent.com/j2store/doc-images/master/set-up/currency/currency\_decimal\_separator.png)

**Video tutorial**

{% embed url="https://youtu.be/MXMywDaUErw" %}
How to change decimal separator using currency settings
{% endembed %}

****
