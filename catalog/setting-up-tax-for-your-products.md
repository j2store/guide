# Setting up tax for your products

## Requirement for the tax to take effect: <a href="#requirement-for-the-tax-to-take-effect" id="requirement-for-the-tax-to-take-effect"></a>

* Geozone has to be set up for which the tax has to apply.
* Tax rate has to be set up.
* Tax profile has to be created.
* Tax rate has to be associated with the tax profile.
* Tax profile has to be assigned to the products for which tax has to be levied.

## Instance: <a href="#instance" id="instance"></a>

Tax geozone: USA

Tax rate: 10%

Tax profile name: US-TAX

**Steps:**&#x20;

* Navigate to J2Store->Localisation->Geozones and create a new geozone.

![Creating a new geozone](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/setting-up-tax-for-your-products/setting-tax-new-geozone.png)

* Type in a name for the geozone, add the countries for which the tax has to be applied.
* Case A: Apply tax only for few zones within USA.

&#x20;&#x20;

![Filling in details on the newly created geozone](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/setting-up-tax-for-your-products/setting-tax-geozone-details.png)

2\. Case B: Apply tax for all zones within USA.

![Adding country](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/setting-up-tax-for-your-products/setting-tax-adding-country.png)

Navigate to J2Store-> Localisation->Tax rates->Click new.

![](../.gitbook/assets/setting-tax-adding-tax-profile.png)

Fill in the name, tax percentage, geozone and publish the tax rate.

![](../.gitbook/assets/setting-tax-rate-details.png)

Navigate to J2Store->Localisation->Tax profile->New.

![](../.gitbook/assets/setting-tax-adding-tax-profile.png)

Fill in the profile name, set the status and map the tax rate on the profile, choose the associated address.

![Adding details to tax profiles](https://raw.githubusercontent.com/j2store/doc-images/master/catalog/setting-up-tax-for-your-products/setting-tax-tax-profile-details.png)

Navigate to J2Store->Catalog->Products(Or Content->Articles).

![](../.gitbook/assets/setting-tax-nav-to-pro.png)

Edit the products for which you wish to collect tax. Navigate to the J2Store cart tab. Choose the tax profile and save.

![](../.gitbook/assets/setting-tax-profile-in-pro.png)

Frontend:

![](../.gitbook/assets/setting-tax-front.png)

![](../.gitbook/assets/setting-tax-in-cart-page.png)

Thus tax would be levied on the product as per the configuration.

### Issues: <a href="#issues" id="issues"></a>

Please refer the following list of troubleshooting steps:

[click here](https://docs.j2store.org/catalog/setting-up-tax-for-your-products/\[http://docs.j2store.org/troubleshooting-guide/troubleshooting-tax-issues]\(%3Chttp:/docs.j2store.org/troubleshooting-guide/troubleshooting-tax-issues%3E\))

