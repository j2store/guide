# Troubleshooting Tax Issues

## How to display Prices without including tax? <a id="how-to-display-prices-without-including-tax"></a>

Go to J2Store -&gt; Configuration -&gt; Tax tab.

Select No, I will enter prices exclusive of tax to Prices Entered With Tax option.

Select Excluding tax for both Display prices in product pages and Display prices during cart/checkout.

![tax excl](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-tax-issues/tax-excl.png)

## How to display prices with including tax? <a id="how-to-display-prices-with-including-tax"></a>

Go to J2store -&gt; Configuration -&gt; Tax tab.

Select Yes, I will enter prices inclusive of tax to Prices Entered With Tax option.

Select Including tax for both Display prices in product pages and Display prices during cart/checkout.

Set YES to Display tax information below the prices \(in product pages\).

![tax incl](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-tax-issues/tax-incl.png)

## Why the tax rate is not showing up for particular zone? <a id="why-the-tax-rate-is-not-showing-up-for-particular-zone"></a>

For example, do you want to setup the tax rate for california ?

1. First thing is you have to create Geozone for californiaGo to J2store -&gt; Localisation -&gt; Geozones and click NEW button on top left.
2. Enter the Geo Zone Name in the text box.Select Enable.Click on Add Country/Zone button then you will get two dropdowns for choosing country and zone.Choose the country name and zone name from the dropdown list.Click Save & Close.
3. Add the Geozone to the tax rate you have created.. Open the tax rate you have created and the geozone you have created will be listed in the Geo Zone list.

#### Configured all the things properly but still tax is not showing.Why?

You might have missed one most important step. You should add the tax profile to the product.

Open the product, go to J2Store cart and navigate to the general tab.

Add your tax profile created.

![tax prof](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-tax-issues/tax-prof.png)

## Why tax is not displayed when changing the setting of the tax calculation from billing address to the delivery address? <a id="why-tax-is-not-displayed-when-changing-the-setting-of-the-tax-calculation-from-billing-address-to-the-delivery-address"></a>

If you choose shipping address in J2Store Tax configuration then you should also change the associated address to shipping address in the tax profile.

Go to tax profile and set the associate address as shipping address.

## Why tax information is showing as “Excl.tax” even you have chosen including tax in configuration <a id="why-tax-information-is-showing-as-excltax-even-you-have-chosen-including-tax-in-configuration"></a>

Seems to be choosing of wrong default customer address.

In your tax configuration, you might have chosen default customer address as “No address”. Here should choose store address as default customer address.

Because, the guest customers don’t have any billing or shipping address so in this case, it will take default address as store address to display the correct tax information.

## HOW TO Apply tax to all customers comes from world wide? <a id="how-to-apply-tax-to-all-customers-comes-from-world-wide"></a>

It is very simple. Just create one geozone and include all countries.

Go to J2Store &gt; Localisation &gt; GeozonesClick NewEnter Geozone name and choose the status EnabledSave.

After saving, you can see Import countries button. Click Import countries button to import all countries and save.

Now assign this geozone to your tax rate.

## \[How To\]Display tax information with follow link text ? <a id="how-todisplay-tax-information-with-follow-link-text-"></a>

### Step-1 Enable tax information to be displayed on product page <a id="step-1-enable-tax-information-to-be-displayed-on-product-page"></a>

Go to J2Store -&gt; Configuration - Tax settings. Set Display tax information below the prices \(in product pages\) to YES.See the screenshot below

![tax including text](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-tax-issues/tax_including_text.png)

It would display a text like this: \(Incl. XX% tax \)

This might be in English.

You can change this with a language override for below language constantLanguage constant is: J2STORE\_PRICE\_INCLUDING\_TAX

### Step-2 Creating language override <a id="step-2-creating-language-override"></a>

Go to Extensions -&gt; Language\(s\) -&gt; select Overrides.

Choose your language\(For example, English\(en-GB-Administrator\)\) in filter section and click new on top left.

Add J2STORE\_PRICE\_INCLUDING\_TAX in Language constant text box.

In Text box, add Inkl %s MwSt \(add the link using html anchor tag\). For example,

Check For both locations.

Location should be administrator.

Save and close.

Here is a screenshot showing the language override

 Here is how it looks in the front end

![tax override](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-tax-issues/tax_override.png)

![front end](https://raw.githubusercontent.com/j2store/doc-images/master/troubleshooting-guide/troubleshooting-tax-issues/front_end_display.png)

