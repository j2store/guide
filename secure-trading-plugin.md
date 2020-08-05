# Secure Trading Plugin

The J2Store SecureTrading Plugin \(Payment Pages\) requires:

1. PHP Version: 5.2+
2. Joomla 2.5 +
3. J2Store 2.0+

**2.1. Installation** Installation of the plugin is extremely simple.Use the default Joomla installer to install it

**2.2. Configuration** To configure the plugin you should perform the following steps:

1. Head again to ‘Joomla Admin’ - ‘Extensions Manager’ - ‘Plugin Manager’.
2. Locate ‘SecureTrading Payments’ and open it.
3. A list of options will now appear. Configure these to your liking and then click ‘Save’.

**Payment option title** - Enter a name that will appear in the payment option section in the checkout.

**SecureTrading Site Reference** - Site reference provided by the Secure Trading.

**Settlement Status** - This is the settlement status that will be applied to all successful transactions. The default status is “0”.

**Settlement Due Date** - This is the number of days you wish to wait before retrieving funds from your customers’ account. The default value is “Process Immediately”.

**Site Security Password** - This is used to generate the Site Security hash. This option is discussed further in section 2.5.

**Use Notification service** - Select this option to enable the notification service. This option is discussed further in section 2.6.

**Notification Password** - This is the notification hash. This option is discussed further in section 2.6.

**2.3. Notification** You must set-up a notification in MyST before this plugin can work correctly.

This feature is responsible for updating order information in the J2Store back-end after payment has been made via the SecureTrading Payment Gateway.

To set-up a notification you should perform the following steps:

* Login to MyST and select “Notifications”.
* Select ‘Add Filter’ and then enter the following information:

**FILTERS**

**Description:** Enter a recognizable name of your choice here.

**Requests:** Auth

**Payment Types:** Select all card types that you will be accepting here.

**Error Codes:** All Error Codes

* Click ‘Save’.
* Select ‘Add Destination’ and enter the following information:

**DESTINATIONS**

**Description:** Enter a recognizable name of your choice here.

**Notification Type:** URL

**Process Notification:** Online

NOTE: replace your_domain_name.com in the url with your domain name.

**Security Password:** This is the field that you will enter your chosen notification password into. See section 2.6 for more information.

**Security Algorithm:sha256**

**Fields:**

* errorcode
* orderreference
* securityresponseaddress
* securityresponsepostcode
* securityresponsesecuritycode
* status
* transactionreference

**Custom Fields:** None

1. Click ‘Save’.
2. Select the filter and destination you have just created from the two initially blank select menus \(under ‘Current Notifications’\).
3. Click ‘Save’.

The notification will now have been enabled.

**2.4. Redirect** You must set-up a redirect before this plugin will work correctly.

Please complete the Redirect Form and email it to our support department at&lt;link-text url =“support@securetrading.com”target =“\_blank”rel = “noopener”&gt; click here

The Redirect Form can be downloaded here: [click here](http://securetrading.com/sites/default/files/downloads/ppages/STPP_Redirect_Request_Form.doc)

The following information should be inserted into the redirect form:

**Redirect URL:**http://your\_domain\_name.com/index.php?option=com\_j2store&view=checkout&task=confirmPayment&orderpayment\_type=payment\_securetrading&paction=display\_message” target = “\_blank”rel = “noopener”&gt; click here

NOTE: replace your_domain_name.com in the url with your domain name.

**Fields:** None

**Custom Fields:** None

**2.5. Site Security**

A security code will prevent malicious users from modifying sensitive payment information before being directed to the payment screen.

This feature can be enabled by following these steps:

1. Head to the Securetrading plugin configuration \(‘Joomla Admin”Extensions Manager”Plugin Manager’ - ‘SecureTraing Payments’ - ‘Edit’\).
2. Enter a hard to guess combination of letters and numbers into the ‘Site Security Password’ field. This combination should be at least 8 characters long.
3. Click ‘save’.
4. You must now contact Support by emailing\[email protected\]”target = “\_blank” rel = “noopener”&gt; click here Inform them that you have “enabled the Site Security Password Hash”. When prompted for a list of “enabled fields”, you must tell themthe following, in this order:currencyiso3amainamountsitereferencesettlestatussettleduedatePASSWORD \*

‘Site Security’ is now enabled. Remember to never tell any other individuals your Site Security Password. Do not store hard copies of this password anywhere.

> The last field, ‘PASSWORD’, is to be the combination of characters you entered into the ‘Site Security Password’.

**2.6. Notification Hash** It is highly recommended that you enable the notification hash. See section 2.3 for more information on the notification script itself.

To enable the notification hash you will firstly have to enter a ‘Security Password’ in the ‘Destination’ window of the MyST Notification page \(see section 2.3\).You will also have to enter the same password into the J2Store SecureTrading Payment Plugin configuration page. Details on how to configure the plugin were given in section 2.2.

**2.7. Expected Behaviour** Successful orders will be set to the ‘Confirmed Status’.

Declined transactions will be set to the ‘Failed Order Status’.

Failed transactions will be set to the ‘Failed Order Status’.

Raw transaction details can be viewed by clicking the View button on the Order details page \(Joomla admin-&gt;J2Store-&gt;Orders and click an order ID to go to the details page\)

