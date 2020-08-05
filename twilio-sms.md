# Twilio SMS

Now you can integrate Trilio in your online store. With Trilio you can send SMS alerts to mobile regarding the status of orders to your customers. You can also enable the app to send notifications store owner when a new order is made.

**Requirements**

* PHP 5.4 or higher
* Joomla 3.3 or above
* J2Store 3.2.x or above

**Installation**

1. Use the joomla installer to install the app.
2. In the backend, go to J2Store &gt; Dashboard &gt; Apps.
3. Click Enable in the TwilioSMS app as shown in the image below. 

![st01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/twilio-sms/smstwilio01.png)

4. Once app is enabled, click open to setup the Basic settings of the app.

![st01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/twilio-sms/smstwilio01.png)

![st02](https://raw.githubusercontent.com/j2store/doc-images/master/apps/twilio-sms/smstwilio02.png)

**Basic Settings**

**Account id\(SID\):** Enter the valid Account ID provided by the Twilio.

**Token:** Enter the valid token provided by the Twilio.

**From Phone number/ short code:** Enter the value \(Phone number\) from which the message should send to all customers.

**When message will send:** Choose when the message should send. Select either After payment complete or After status update.

**Custom field of Phone number:** Select the receiver’s phone number. If you choose phone\_2, then the SMS will be sent to the customer’s number entered in the field Mobile in the checkout.

**Send message to admin:** Select YES will enable sending SMS to admin.

**Admin Mobile:** Enter the valid mobile number of admin.

**Admin message:** The value entered here will be displayed as body of the message when admin receives. You can use the shortcodes mention in the top of the backend app settings.

**User Message:** The value entered here will be displayed as body of the message when user / customer receives. You can use the shortcodes mention in the top of the backend app settings.

![st03](https://raw.githubusercontent.com/j2store/doc-images/master/apps/twilio-sms/smstwilio03.png)

![st04](https://raw.githubusercontent.com/j2store/doc-images/master/apps/twilio-sms/smstwilio04.png)

