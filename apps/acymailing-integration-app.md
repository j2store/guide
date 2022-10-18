# AcyMailing Integration App

## Requirements <a href="#requirements" id="requirements"></a>

* PHP 5.2 or higher
* Joomla 3.3 or above
* J2Store 3.1.6 or above

## Installation Instructions <a href="#installation-instructions" id="installation-instructions"></a>

1. Use the Joomla installer to install the app.
2. In the backend, go to J2Store Dashboard -> Apps as shown in the image below.

![ai01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/acymailing-integration-app/am1.png)

3\. Click Enable in the Acymailing plugin. (type=j2store).

&#x20;

![ai02](https://raw.githubusercontent.com/j2store/doc-images/master/apps/acymailing-integration-app/am2.png)

4\. After the app is enabled, click on Open to set the configuration for the app.

![ai03](https://raw.githubusercontent.com/j2store/doc-images/master/apps/acymailing-integration-app/am3.png)

5\. Enter the parameters (read the explanation about each parameter given below)

6\. Save and close it.

## Parameters <a href="#parameters" id="parameters"></a>

The below image illustrates the settings of parameters:

![ai04](https://raw.githubusercontent.com/j2store/doc-images/master/apps/acymailing-integration-app/am4.png)

1. Acymailing List -This option is used to display all your Acymailing subscribers list. You can select multiple lists in this option.

![ai05](https://raw.githubusercontent.com/j2store/doc-images/master/apps/acymailing-integration-app/am5.png)

2\. Acymailing List Title -The text entered here will be displayed when customer is about to select payment method. If you use a muliti-lingual site, language constants can be entered here and then language over-ride can be made.

3\. Auto Subscription - If you enable this by choosing Yes, then the customer will be automatically added to subscribers’ list. A confirmation email will be sent to the customer. All this will be done on successful order placement.

4\. Display Auto subscription in products -If you enable this option, then a check box will appear in both the back end and front end. This is to offer product specific subscription. Consider the image below:If you check this option, then it will override the previous ‘Auto Subscription’ option.

![ai06](https://raw.githubusercontent.com/j2store/doc-images/master/apps/acymailing-integration-app/am6.png)

## Front end view of Auto Subsctiption <a href="#front-end-view-of-auto-subsctiption" id="front-end-view-of-auto-subsctiption"></a>

Below image illustrates the cart view, in which one can see the items that are added to the cart. If any change is needed, it can be done before checking out.

&#x20;

![ai07](https://raw.githubusercontent.com/j2store/doc-images/master/apps/acymailing-integration-app/am7.png)

In the front end, if you add your desired product to the cart and proceed to checkout, then you will see the auto subscription status. It will reflect your settings in your product configuration.

Consider the below image:

![ai08](https://raw.githubusercontent.com/j2store/doc-images/master/apps/acymailing-integration-app/am8.png)

The image shows the options for subscriptions. If you have **Enabled** Auto Subscription, and **Disabled** Display Auto Subscription in products, then you will not get any options here.
