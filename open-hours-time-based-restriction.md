# Open hours \(time based restriction\)

Open hours app allows you to restrict orders from customers based on your store’s operational timings. You can configure your store’s opening and closing time for all days of the week. This means any orders coming in after closing hours will not be accepted.

Make sure that you set the 24hr format for time configuration.

**Requirements**

* PHP 5.4 or higher
* Joomla 3.3 or above
* J2Store 3.2.x or above

**Installation**

1. Download the app package from our site’s extensions section and install it using Joomla installer.
2. After installing the app, go to J2Store &gt; Apps and click Enable on the app named “Opening hours”.
3. Once activated, click on open to configure your store opening and closing time.

**Basic settings**

**Error message**

This is the place to show error message when the customer places an order outside the store’s operational timing.

Enter your custom error message here. You may also enter a language string and write a langugage override.

For eg: Sorry ! Orders are accepted only after %s and Before %s.The first %s will be from time and second %s will be to time in the below configuration.

**Shop available time**

For instance, if your store’s operational timing is from 10.00 am to 11.00 pm on weekdays and closed on weekends \(Saturday and Sunday\), you will have to configure your store timing like below,

**On weekdays**

From time - 10.00

To time - 23.00

![oh01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/open%20hours/oh_01.png)

Now if customer tries to place an order before opening time or after closing time on weekdays, the customer will be displayed with a message to inform that orders cannot be placed right now.

**On weekends**

To set shop closed on weekends \(Saturday and Sunday\), you will have to set just 1 minute for saturday - sunday. Refer below image,

![oh02](https://raw.githubusercontent.com/j2store/doc-images/master/apps/open%20hours/oh_02.png)

If customer tries to purchase on weekends, he will be informed that orders cannot be placed.

![oh03](https://raw.githubusercontent.com/j2store/doc-images/master/apps/open%20hours/oh_03.png)

