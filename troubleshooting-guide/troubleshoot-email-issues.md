# Troubleshooting Email Issues

Mail delivery is a bit tricky process and it primarily depends on your hosting service. Yes. You read it right. Neither Joomla or J2Store cannot send an email. They can only prepare the email and pass it to the mail server of your hosting service \(or an SMTP service\)

The role of J2Store in the mail notification is just to prepare the email message and the subject and pass on to Joomla’s mail handler \( JMail class \) Even Joomla cannot send emails. Yes. That is correct. The email sending has to be handled by a mail server \(your Hosting service\). So even Joomla passes on the message to your mail server.

It is your mail server \(hosting server\) that sends out the mail. Similarly, at the receiving end, another mail server receives it.

Applications like J2Store or Joomla have very little control over the mail delivery. They can only initiate the sending process. Once done, the mail server takes over.There could be hundreds of reasons why an email was not received by a person. 

The receiving mail server might have anti-spam filters \(like GoDaddy\), firewall, and other processing rules. And there is no way of checking whether mail deliver got failed \(called bounce\) by the application. 

However, if a mail bounces, a mail delivery failure message is sent to the inbox of the From email \(the from email you set in the Joomla -&gt; Global configuration - Server settings -&gt; Mail settings\)

Here is a simple explanation how Joomla extensions including J2Store uses the Joomla’s mailing capability [click here](https://www.ostraining.com/blog/how-tos/development/how-to-send-email-from-your-joomla-extension/)

J2Store uses the Joomla’s default mail wrapper \(JMail\) class for sending the order notifications to the store administrator and the customers.

There can be a number of reasons why a customer or the store administration has not received the emails. The following are a few scenarios and solutions.

#### **Is your Joomla mail server working?**

You can check this by creating new user with valid email address. Joomla usually sends an email notification about the account creation.Also try sending a test email from the Joomla global configuration.If you can’t get any default Joomla emails to work, the settings at your mail server are incorrect.

#### **Mail not receives on placing order but receives when notifying from backend ?**

It is mainly due to Mail function is disabled in PHP setting or it is disabled by your hosting provider.

#### **Is your site in localhost?**

In this case, you won’t receive any emails. Please host your site with a web hosting service provider. 

#### **Did you set up the ‘From’ email and Admin email in shop settings**

**Version 2.x:** Go to Joomla admin -&gt; J2StoreOptions - Shop settingsSet your Default From email and the Admin Email there. 

**IMPORTANT:** Make sure that your ‘From’ email and the Admin email are different.

**For Version 3.x:** Go to Joomla admin - Global Configuration - Server tab. Check your From email and other mail settings.

Then go to J2Store - Configuration - store settings.

#### **Make sure the Store administrator email is not same as the From email set in the global configuration.**

Many email servers and clients will flag an email as spam if the ‘From’ email and the admin email are the same. So using two different emails solves the problem.

Example: If your from email id is: **myemail1@gmail.com**, then your Admin email could be **someothermail@gmail.com.**

#### What is the status of the order?

Most of the Payment Plugins for J2Store are configured to send an order notification to the administrator and the customer, only when the order status is CONFIRMED.

 However, a few plugins such as Bank transfer, Cash on Delivery, Money Transfer, Offline Payment plugins, will send the notification for all order statuses.

So if you are not receiving an email, then check the status of the order.

 Most of the Payment gateways send a feedback after a customer makes a payment successfully. 

Based on the feedback received, the Payment plugins set the order status and trigger the email. Occasionally, the payment gateways may not send the feedback or it may not reach your server for a variety of reasons. For those reasons, email might not be sent.

#### Mail server issues

Sometimes, your host mail server may have issues. It might not send the emails. 

Here is an easy way to find out if your mail server has an issue:

* Go to Joomla admin -&gt; User Manager. 
* Create a new user by entering a valid email. 
* If you did not receive any notification about the new user creation, then your mail server has an issue.
* Contact your hosting service provider. They will help you out.

#### Customer receiving the email, but the store administrator is not getting or vice versa.

If this issue occurs, then J2Store is successfully sending the order notifications using Joomla mail functions. 

No problems with your Joomla installation.

The problem is with the customer’s or the administrator’s email. 

Ask your customer / store administrator to check their SPAM folders. If still not there, contact your hosting service provider.

#### Is your site hosted in GoDaddy?

* If you are using GoDaddy as your hosting service provider and did not receive the email, then change the subject of your email template. 
* This broken host introduced unreasonable email filters recently, which prevent sending order notification emails. Refer this [click here](https://www.j2store.org/forum/2-general-questions/5036-solved-order-email-sending-problems-with-godaddy.html)

Still have issues ? Please reach out to us via the support form or ticket system.

