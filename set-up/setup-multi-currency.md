# Set up multi-currency

**J2Store Multi Currency**

J2Store multi currency feature allows store owner to setup multiple currencies. For example, if the location of store is United States and the store owner wants his store to be accessed by customers from Japan and European countries, then he / she will have to create one primary currency \(for united states\) and two secondary currencies \(one for Japan and other for European countries\).

## How to setup Primary or default currency? <a id="how-to-setup-primary-or-default-currency"></a>

First you have to decide your primary or default currency for your store. The **value** option in currency settings is used to set the default currency. If the value is set be 1.000000 for a particular currency, it will serve as the default currency.

For e.g., if US $ is been set the value 1, it will be the default currency and the corresponding value will be 0.81 for Euro. In this way J2Store will calculate the prices for products based on currency transitions.

To make the currency value auto update, go to **J2Store &gt; Configuration &gt; Store tab** and choose **YES** to Auto Update Currency.

![Autoupdate currency](https://raw.githubusercontent.com/j2store/doc-images/master/set-up/set-up-multi-currency/multi-currency_autoupdatecurrency.png) Choose the Default Currency as **USD** in your store configuration.

After choosing Auto update currency to YES, when you are going to create secondary currency, the value of the currency will be updated automatically. See the below picture, ![Value of available currencies](https://raw.githubusercontent.com/j2store/doc-images/master/set-up/set-up-multi-currency/multi-currency_value.png)

## J2Store Currency Switcher <a id="j2store-currency-switcher"></a>

Go to Extension &gt; Modules.

Find the J2Store currency module and enable it.

Open the module, set the module position to any one of your template’s positions.

Assign it to the All pages or to the particular menu and Save it.

![Currency setup](https://raw.githubusercontent.com/j2store/doc-images/master/set-up/set-up-multi-currency/multicurrency_currency.png)

**Frontend** ![Frontend view](https://raw.githubusercontent.com/j2store/doc-images/master/set-up/set-up-multi-currency/multi-currency_frontend.png)

**Video Tutorial:** Here is a video that would assist you on setting up multi-currency on your site:

{% embed url="https://youtu.be/uLw-iEkJkFk" %}





