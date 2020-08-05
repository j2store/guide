# Recommended Tax configuration for US States

This is an example setting for stores in United States. This also applies to many other countries that follow a US style of tax system. For detailed information on tax, please consult an expert.

**Note:** Current US law requires you to collect taxes where you have an interest/ongoing concern — that is, where you have physical stores, distribution centers, headquarters, and so on. For many online stores there is only one location. However, if you have stores that operate in many states or countries, or if you have revenues exceeding approximately $2M per year, we recommend that you use a third-party tax provider because there can be a considerable number of tax rules and tax zones to manage.

**Important:** No guarantee is offered with respect to any of the information given here. Please contact an expert before you take any decisions about tax matters

**NOTE:**The example given below, assumes you have a store in Texas and you charge 8.5% tax on the goods sold to customers in Texas. All customers coming from other states are NOT taxed

## Step 1 : Create a geozone for Texas <a id="step-1--create-a-geozone-for-texas"></a>

Go to Localisation -&gt; Geozones -&gt; New

**Geozone Name:** Texas Zone

**Country :** United States

**Zone :** Texas

## Step 2: Create a tax rate <a id="step-2-create-a-tax-rate"></a>

Go to Localisation -&gt; Tax Rates -&gt; New

**Name :** Sales Tax \(you can give any name here\)

**Tax Percent :** 8.5

**Geozone :** Texas Zone

**Status :** Published

## Step 3: Create a tax profile and rules <a id="step-3-create-a-tax-profile-and-rules"></a>

Go to Localisation -&gt; Tax Profiles -&gt; New

**Name:** Default Tax Class

**Enabled:** Yes

**Tax rules**

Click Add

**Rate:** Sales Tax

\*\*Associated Address: \*\* Shipping

## Step 4: Configure tax settings <a id="step-4-configure-tax-settings"></a>

Go to Set up -&gt; Configuration -&gt; Tax

**Prices Entered with Tax:** No, i will enter prices EXCLUSIVE of tax

**Calculate tax based on:** Shipping address

**Default Customer address:** Store address

**Display prices in product pages:** Excluding tax

**Display prices in cart / checkout :** Excluding tax

**Apply discounts :** Before tax

Save.

## Step 5: Create a product and choose the tax profile <a id="step-5-create-a-product-and-choose-the-tax-profile"></a>

J2Store uses Joomla articles as products. So go to Article Manager and create a New Article / Product \(If you sue any other catalog source like Zoo or Sebold, you should head there\).

Product creation steps are explained under the topic **Products**.

Here let us just see how to choose the tax profile

Go to J2Store Cart tab -&gt; General tab

**Tax Profile :** Default tax class

![Default tax-rate-for-Us-stores](https://raw.githubusercontent.com/j2store/doc-images/master/tax-configuration/Recommended-for-US-stores/Tax-config-default-tax-rate.png)

**IMPORTANT** If you do not choose the tax profile, then tax will not apply in the store front.

**Video Tutorial:**

{% embed url="https://youtu.be/n1sZ5Udbm3Q" %}

\*\*\*\*

