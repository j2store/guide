# Tax Utilities

The app provides a one-stop configuration for the tax set up. The tax utilities app is a replacement of the following apps.

* Tax display
* Combine taxes
* Tax exemption

1. Store-wide tax emeption

2. Certificate based tax exemption

* User group-specific tax rates

## Installation <a id="installation"></a>

You could download the app from the My downloads section under the My account menu of the J2Store site and install it on your site using the Joomla default installer. Once installed, the app can be enabled and configured under J2Store-&gt;Apps.

## Configuration <a id="configuration"></a>

Since the app is a combined form of the above mentioned apps, it has 5 tabs for each functionality it offers. This is how you could set this app up.

## Tax display <a id="tax-display"></a>

This tab allows you to choose whether you would display the product price inclusive or exclusive of the tax based on the user groups, where you wish to display the tax, restrict\(hide or show\) the tax display based on the user groups.

The following are the parameters that have to be set up to customize your tax display. \*\*NOTE: The settings set here would override the default tax configuration under J2store-&gt;Setup-&gt;Configuration-&gt;Tax. \*\*

* **Would you like to control how taxes show in the product/cart pages?**

Set this option to Yes if you wish to control how tax is shown on the product or cart pages. The value chosen in this field determines whether or not the following parameters take effect. For example if you select Disable to this option, the options that follow wouldn’t have any effect.

**Where should the tax be displayed?**

This option lets you choose the place where the tax display settings should take effect. The values available are Product view and cart view.

When you choose the product view, the following options that restrict tax display would take effect only on the product page, that is on the item view and list view.

When you choose the cart view, the following options that control tax display would affect only the cart page.

You could also choose both the options if you wish to display tax based on the options that follow on both the product view and the cart page.

* **Chosen user groups will see prices excluding tax in product pages**

Select the user groups for which you wish that the product price should exclude the tax on the product page. For instance, if you select Wholesale user group here, then when users of the wholesale user group login to the site, they would be seeing price without tax on the product page.

NOTE: This option affects only the product page. Leaving this field empty would disable the option.

**Chosen user groups will see prices including tax in product pages**

Select the user groups for which you wish to display the product prices inclusive of the tax on the product page. For instance, if you select the Registered user group here, the users of that group would view the product price inclusive of the tax in the product page.

NOTE: Setting only affects product page. Leaving this field empty would disable the option.

**Tax should not be calculated to the following user groups in cart page**

The user groups chosen in this option would not have tax calculated on the cart page, that is they would be exempted from the tax calculation. For instance, if the Guest user group is chosen in this option, the guest users would not have tax applied to their cart. They would have product prices exclusive of tax

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/taxpage.png)

\*\*Working: \*\*

**For wholesale users:** With the above set up, the users of the wholesale group would see product prices excluding tax on the product page, regardless of the setting on the J2Store configuration.

**For registered users:** With the above set up, the registered users would see product prices including tax on the product page, irrespective of the setting on the J2Store configuration.

\*\* For guest users:\*\* Users of the guest group would be exempted from tax on the cart and checkout pages.

**J2store Configuration**

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/j2storeconfiguration.png)

**For whole sale users**

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/wholesaleusers.png)

**For registered users**

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/registeredusers.png)

**For guest users**

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/Guestusers.png)

## Combine taxes: <a id="combine-taxes"></a>

This tab would provide settings for you to combine all form of taxes on your site.

**Would you like to combine the taxes in the totals column** Set this to enable if you wish that all the taxes\(Tax for product, tax for shipping\) should be combined together and shown at the totals section.

**Label for the combined taxes** What should be the label when taxes are combined and shown at the totals section. Mention that label here.

\*\*Instead of combining the shipping tax with the product taxes, add it to the shipping cost \*\*

When you set this option to Yes, the tax of the product would be shown separately while the tax on shipping would be included in the shipping cost itself.

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/taxutilities.png)

**Working:**

With the above set up, the tax rates at the cart page would be shown like this:

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/working.png)

## Store wide tax and exemption: <a id="store-wide-tax-and-exemption"></a>

This would allow you to force tax calculation based on the address of the store mentioned under J2Store-&gt;Setup-&gt;Configuration-&gt;Store. Irrespective of the address entered by the user, tax would be displayed based on the store address.

\*\*Force tax to be calculated on store address for ALL Customers \(ignore customer address\)? \*\*

Set this option to Yes if you wish that tax has to be calculated based on the store address and not the user’s address.

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/App-tax-utilities.png)

NOTE: This setting has to be turned on only when you wish that users have to be levied tax irrespective of their address.

**Working:** Store address: UK. Tax is set for: UK. Customer address: None or any other address other than UK. Tax: UK tax would be levied on all users irrespective of their address.

**Tax setup:**

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/taxsetup.png)

\*\*Store address: \*\*

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/storeaddress.png)

\*\*User address and tax calculation at frontend: \*\*

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/useraddressandtaxcalculation.png)

## Certificate based tax exemption <a id="certificate-based-tax-exemption"></a>

 Enabling this option would enable users to be exempted from tax once they upload a file\(tax exemption certificate\) at the checkout page during registration.

**Provide certificate based tax exemption**

Enabling this option would display a checkbox asking users to upload a tax exemption certificate during registration. The file uploaded by users would be available for store administrators to download at the order history of that particular order.

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/certifictaebasedtax.png)

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/certicatebasedtax2.png)

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/invoice.png)

## Tax rate per user group <a id="tax-rate-per-user-group"></a>

 This tab has provisions to help you set up user group based tax rates.

**User group based tax rates**

Enable this option to set up tax rates based on user groups. The available tax rates and user groups would be listed and you could map them accordingly.

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/usergroupbasedtax.png)

**Working**

 

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/usergroupbasedtaxworking.png)

![](https://raw.githubusercontent.com/j2store/doc-images/master/apps/tax-utilities/usergroupbasedtax2.png)



