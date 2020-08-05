# Shipstation

The new J2Store integration with Shipstation helps you to integrate your J2Store site with one of the best shipping solution, Shipstation. Now import your orders and manage shipping on the go with the help of this integration. With Shipstation, you need not worry about shipping your orders using different carriers, cause you can manage everything at a one stop place using this integration.

Shipstation is a multi-channel, multi-carrier shipping solution that simplifies the shipping process for online merchants. Shipstation can be integrated seamlessly with any shipping carrier and channel and your orders can be easily tracked and managed with just few clicks, regardless of the location.

Now conduct your business with more fluidity and transparency with the easy interfacing of shipstation.

NOTE: Shipstation will not send any Webhook notifications when you manually mark an order as Shipped in your ShipStation console. It is treated as externally fullfilled orders. Tracking numbers for those orders should be entered manually in your ShipStation and also in J2Store.

**Installation**

The integration can be downloaded from our site and installed using the default joomla installer.

**Pre-requisites**

A shipstation account is required to use the integration.You could create one at www.shipstation.com

**Creating an account and generating API keys**

To get the API keys for the integration, it is necessary to create an account with Shipstation.Following are the steps to be done:

* Go to www.shipstation.com.
* Click on the Start your 30 day free trial button.
* A page appears asking you to create a new account. Furnish your details and click on the Lets go to shipping button.
* Before logging into your account, it is necessary to verify the email address by clicking on the link sent to your registered email address.
* Post verification, you can login to the account by clicking on the login button on the top right corner and keying in the credentials.
* Click on the settings icon on the right corner.
* There will be lot of tabs displayed on the left side. Click on the Account tab.
* Clicking on the Account tab will open up the options from which the API settings option has to be chosen.
* Click on the Generate API keys button. API keys will be generated.

The below screenshots are for reference:

**Creating an account with Shipstation**

 

![ss01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/shipstation/shipstation01.png)

**Generating API keys** 

![ss02](https://raw.githubusercontent.com/j2store/doc-images/master/apps/shipstation/shipstation02.png)

![ss03](https://raw.githubusercontent.com/j2store/doc-images/master/apps/shipstation/shipstation03.png)

![ss04](https://raw.githubusercontent.com/j2store/doc-images/master/apps/shipstation/shipstation04.png)

![ss05](https://raw.githubusercontent.com/j2store/doc-images/master/apps/shipstation/shipstation05.png)

**Webhook URL**

After entering the API keys in the app, the next step would be to set up the webhook URL in the Shipstation account.

This has to be done in order to receive notifications of the changes that occur in shipstation. The notifications will come up in your J2Store site’s backend.So this is more of a synchronization.

**Setting up webhook notifications**

Webhook notifications can be set up by following the steps given below:

* The URL for webhook can be fetched from the app’s settings. 

![ss06](https://raw.githubusercontent.com/j2store/doc-images/master/apps/shipstation/shipstation06.png)



* Now login to your Shipstation account.
* Go to Settings-&gt;Integrations-&gt;Integration partner-&gt;Webhook.
* Specify the URL in the field Webhook URL and save.

 **App settings**

![ss07](https://raw.githubusercontent.com/j2store/doc-images/master/apps/shipstation/shipstation07.png)

The following are the parameters that have to be filled for the integration to work:

* **API key:** The shipstation API key has to be specified here. The procedure to generate the API keys has been mentioned here
* **API Secret** The shipstation secret key has to be mentioned [here](http://docs.j2store.org/articles/2093085-shipstation#apikeys).
* **Webhook URLThe webhook URL** to be specified in the shipstation account’s integrations part is provided here.
* **Allowed Order status** The orders with the chosen status will be synchronized with Shipstation. For example if the status is chosen as Confirmed here, then all the orders whose status is confirmed will be synchronized with Shipstation.
* **Debug** This option has to be set to Yes if the activity of shipstation has to be logged.

![ss08](https://raw.githubusercontent.com/j2store/doc-images/master/apps/shipstation/shipstation08.png)

