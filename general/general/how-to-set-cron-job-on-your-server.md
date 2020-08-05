# How to set cron job on your server

Do you don’t know how to set cron job on your server ? Our guide here helps you to set cron job on your server.

## Identify cron security key <a id="identify-cron-security-key"></a>

Starting from J2Store 3.2.20, we are supporting a cron job. This system, at the moment, is not used by the J2Store core functions. However a few apps are using it.

You can find the cron security key in your store settings.

Go to J2Store &gt; Setup &gt; Configuration &gt; Store tabYou can see the security key for running cron jobs. Click on Regenerate button to generate new key. Please see the below image

![Cron key](https://raw.githubusercontent.com/j2store/doc-images/master/general/security%20key%20for%20running%20cron%20job.png)

This security key can be used for execution of cron jobs required by apps and plugins. This will ensure only legitimate requests are allowed and executed. The cron requests without this key will be denied access.

## Create cron job via cPanel <a id="create-cron-job-via-cpanel"></a>

* Go and login into your cPanel
* In the Advanced section of the cPanel, Click Cron Jobs

 

![Intro](https://raw.githubusercontent.com/j2store/doc-images/master/general/advanced.png)

* Under Cron Email, type the e-mail address that you want to receive notifications, and then click Update Email. Every time the cron job runs, the e-mail account will receive a message.
* Under Add New Cron Job, enter the interval for the command that you want. If you select an interval option under Common Settings, cPanel fills in the values automatically.
* Common Settings — This menu allows you to select a commonly-used interval. The system will configure the appropriate settings in the Minute, Hour, Day, Month, and Weekday text boxes for you.If the wildcard characters \(star\)and intervals confuse you, this menu is an excellent way to learn how to configure the other fields.
* Minute — Select the number of minutes between each time the cron job runs, or the minute of each hour on which you wish to run the cron job.
* Hour — Select the number of hours between each time the cron job runs, or the hour of each day on which you wish to run the cron job.
* Day — Select the number of days between each time the cron job runs, or the day of the month on which you wish to run the cron job.
* Month — Select the number of months between each time the cron job runs, or the month of the year in which you wish to run the cron job.
* Weekday — Select the days of the week on which you wish to run the cron job. In the Command text box, type the command that you want to run. For example if you wants to run a cron job request for renewing / expire subscriptions in our Subscription and Memberships app, enter like below

```text
wget -O /dev/null "http://www.example.com/index.php?option=com_j2store&view=cron&command=appsubscriptionproduct&cron_secret=XXXXX" > /dev/null
```

Where XXXXX is your cron secret key. Replace www.example.com with your domain nam\*\*\*

* Click Add New Cron Job. \*\*You can also use one of the following commands depending on your server:

**Linux System\*\***

```text
lynx -source "http://www.example.com/index.php?option=com_j2store&view=cron&command=appsubscriptionproduct&cron_secret=XXXXX" > /dev/null
```

Or

```text
wget -O /dev/null "http://www.example.com/index.php?option=com_j2store&view=cron&command=appsubscriptionproduct&cron_secret=XXXXX" > /dev/null
```

If you access your website using an **httpS protocol**, you may want to use this command instead:

```text
wget --no-check-certificate -O /dev/null "http://www.example.com/index.php?option=com_j2store&view=cron&command=appsubscriptionproduct&cron_secret=XXXXX" > /dev/null
```

Some hosting company block the lynx and wget command in which case you should use the curl one

```text
curl --silent --compressed "http://www.example.com/index.php?option=com_j2store&view=cron&command=appsubscriptionproduct&cron_secret=XXXXX" > /dev/null 2>&1
```

You can also contact your hosting provider and ask them to guide you to set cron job.

