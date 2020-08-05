# Recommended Tax configuration for Canadian Stores

This is an example setting for stores in Canada. For detailed information on tax, please consult an expert.

> NOTE:The example given below, assumes you have a store in Canada, Saskatchewan and you charge 5% GST and 5 % Saskatchewan-PST on the goods sold to customers.

## Step 1 : Create a geozone for Texas <a id="step-1--create-a-geozone-for-texas"></a>

Go to Localisation -&gt; Geozones -&gt; New

Geozone Name: Canada geozone

Country : Canada

Zone : \*

## Step 2: Create a tax rate <a id="step-2-create-a-tax-rate"></a>

Go to Localisation -&gt; Tax Rates -&gt; New

Name : Canada-GST

Tax Percent : 5

Geozone : Canada geozone

Status : Published

## Step 3: Create another tax rate for Saskatchewan-PST <a id="step-3-create-another-tax-rate-for-saskatchewan-pst"></a>

Go to Localisation -&gt; Tax Rates -&gt; New

Name : Saskatchewan-PST

Tax Percent : 5

Geozone : Canada geozone

Status : Published

## Step 4: Create a tax profile and rules <a id="step-4-create-a-tax-profile-and-rules"></a>

Go to Localisation -&gt; Tax Profiles -&gt; New

Name: Canada Tax Class

Enabled: Yes

Tax rules

Click Add

Rate: Canada - GST

\*\*Associated Address: \*\* Shipping

Click Add

Rate: Saskatchewan-PST

\*\*Associated Address: \*\* Shipping

## Step 5: Configure tax settings <a id="step-5-configure-tax-settings"></a>

Go to Set up -&gt; Configuration -&gt; Tax

Prices Entered with Tax: No, i will enter prices EXCLUSIVE of tax

Calculate tax based on: Shipping address

Default Customer address: Store address

Display prices in product pages: Excluding tax

Display prices in cart / checkout : Excluding tax

Apply discounts : Before tax

Save.

## Step 6: Create a product and choose the tax profile <a id="step-6-create-a-product-and-choose-the-tax-profile"></a>

J2Store uses Joomla articles as products. So go to Article Manager and create a New Article / Product \(If you sue any other catalog source like Zoo or Sebold, you should head there\).

Product creation steps are explained under the topic Products.

Here let us just see how to choose the tax profile

Go to J2Store Cart tab -&gt; General tab

Tax Profile : Canada Tax Class

IMPORTANT If you do not choose the tax profile, then tax will not apply in the store front.

## Video Tutorial: <a id="video-tutorial"></a>

{% embed url="https://youtu.be/bchu7-Zysb8" %}



