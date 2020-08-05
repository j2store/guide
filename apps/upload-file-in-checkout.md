# Upload file in checkout

Allow customers to upload one or more files during the order. The app will come in handy for store owners selling products like printed materials. The customer can upload an image or PDF to their order.

The store owner can download it from the app’s backend and manage all the uploaded files for an order.

## Requirements <a id="requirements"></a>

* PHP 5.4 or higher
* Joomla 3.3 or above
* J2store 3.2.x or above

## Installation <a id="installation"></a>

1. Use the Joomla installer to install the app.
2. In the backend, go to J2Store Dashboard -&gt; Apps as shown in the image below.
3. Click Enable in the Upload file in checkout app.
4. Once the app is enabled, open the app to configure the settings.

![fu01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/upload%20file%20in%20checkout/file_upload_01.png)

## Configuration <a id="configuration"></a>

**No of file field display**

Enter the number of fields to be displayed in the checkout.

**Display Place**

Choose the place where the upload field should be displayed. You can choose either**Billing** or **Shipping**.

![fu02](https://raw.githubusercontent.com/j2store/doc-images/master/apps/upload%20file%20in%20checkout/file_upload_02.png)

**Display upload file field after?**

The upload file field will be displayed after the checkout fields selected here. For example, if you choose Last name, the field will appear after the field Last name.

**Upload file types**

Add your file format types here. If you don’t have any file formats added here, the app will not allow you to upload the file in that format. For example, if you would like to upload the file in .pdf, make sure that you have added this format in this field.

**Manage uploaded files**

By clicking Order File List button on top of the app’s settings page, you can find all the files uploaded by the customer. It displays the file name with the path where the file locates.

![fu03](https://raw.githubusercontent.com/j2store/doc-images/master/apps/upload%20file%20in%20checkout/file_upload_03.png)

**Shortcodes**

Below shortcodes helps you to notify customer that he / she has attached file in this order.

1. \[ORDERFILE\_NOTIFY\]This shortcode will display just the message or information saying that order contains file attachment.
2. \[ORDERFILE\_LIST\]This shortcode allows you to include download link in email. Use this shortcode in your email template so when customer receives order email, he/she can see the link to download the file that was uploaded.

**Frontend**

![fu04](https://raw.githubusercontent.com/j2store/doc-images/master/apps/upload%20file%20in%20checkout/file_upload_04.png)

