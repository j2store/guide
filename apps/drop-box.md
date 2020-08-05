# Drop-box

Sell your files stored in dropbox with J2Store Joomla eCommerce platform. The app enables you to connect your dropbox and sell the files securely.

**Important Notes**

**NOTE 1:**

The download link sent in the email uses the Dropbox API’s method to create a temporary url.

The API does not allow us to set a custom expiry date \(like in Amazon S3\). Dropbox itself sets the expiry time. The link expires after a few hours.

After the link expires, the customer cannot download using that link. He will have to visit the site, login and then click the Download. This would create another temporary download url and allow the customer to download.

Now there are two ways of solving this

1. You can mention in the email that the link is valid only for a few hours. if it expired, customers have to login to your site to download the file.
2. Dropbox API now allows creating a permanent sharable link. Once created it is valid till your file is removed from dropbox.

You can use the app’s settings to choose whether to send a temporary url or permanent url. In your app’s settings, you can see the following parameter

**Choose the type of link to be included in the email**

* Choose Send a Temporary link if you wants to send temporary link to your customers. This url will expire in few hours.
* Choose Send a Sharable link if you wants to send permanent link. This url never expires unless you delete the shared file in your dropbox account.

**NOTE 2:**

Before proceeding with with setup for the app, make sure you defined a local folder path in J2Store -&gt; Set up -&gt; Configuration -&gt; Basic settings \(example: media \).

**Key features**

* Sell any file stored in Dropbox
* Enables you to retrive the files from the Dropbox remotely.
* Generates a temproary url for the downlodable files, which expires within minutes
* Allows you to control the expiry of the url from settings

**Known Limitations**

* When you are using dropbox for selling digital files, don’t set Download limit and Download expire days. Because these features are not supported by Dropbox API.

**Requirements**

* PHP 5.4 or higher
* Joomla 3.x
* J2Store 3.2.10 or above

**Installation**

1. Download Dropbox app from our site’s extensions section and install it using Joomla Installer.
2. In the backend, go to J2Store &gt; Dashboard &gt; Apps.
3. Click Enable in the Nexmo SMS app as shown in the image below.

![db01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_01.png)

4.\)Once app is enabled, click open to setup the Basic settings of the app.  

![db02](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_02.png)

**How to Generate access token, key and secret key?**

**Step-1:** Go to [https://www.dropbox.com/developers/apps](https://www.dropbox.com/developers/apps) and login using your dropbox account. After logging in, you wil be having the page with Create app. Click on the Create app button. 

![db03](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_03.png)

Step-2: Clicking on Create app button will ask you complete the several steps to create the app.

* Choose Dropbox API as API in your first step of creating app 

![db04](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_04.png)



* Choose your access type.App folderA dedicated folder named after your app is created within the Apps folder of a user’s Dropbox. Your app gets read and write access to this folder only.Full DropboxYou get full access to all the files and folders in a Dropbox.
* Give the name for your app and agree terms and conditions and click create app.

![db05](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_05.png)

Click on Generate button to generate access token for your app.

Step-3: Now the app page will be displayed which contains your \*\*App key \*\*and App Secret key.

![db06](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_06.png)

Step-4: Click on Generate button to generate access token for your app.

  

![db07](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_07.png)

![db08](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_08.png)



Step-5: Copy all the credentials in your notepad and paste it in the J2Store’s dropbox app basic settings.

Basic Settings

**Folder Name:** Enter the name of the folder. The folder will be created\(with the name entered here\) in the path which you have entered in the J2Store configuration. All the files stored in your dropbox account will be fetched and stored in this folder. Access Token: Enter the valid access token for your account provided by Dropbox.

![db09](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_09.png)

**Dropbox Key:** Enter the valid app key associated with your dropbox account.

**Access Token:** Enter the valid access token for your account provided by Dropbox.

**Dropbox secret key:** Enter the valid app secret key associated with your dropbox account. Choosing files in creating digital product

![db10](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_10.png)

1. Once finished configuring basic settings, go to article manager and open your product.
2. Move to J2Store cart tab and then navigate to Files tab
3. Click on Set Product files

![db11](https://raw.githubusercontent.com/j2store/doc-images/master/apps/drop-box/dropbox_11.png)

4.Click on Choose file will display the folder named with the folder name you have given in the basic settings.

5.Choose your file and save.

**Support**

Still have questions? You can post in our support forum: [http://j2store.org/forum/index.html](http://j2store.org/forum/index.html)

Thank you for using our extension.

