# Invoice-prefix-generator

This app allows you to generate a sequential invoice number for orders with **Confirmed** status using the prefix you have entered in the app.

For example, customer adds products to the cart but does not complete the order, but there is still an invoice number generated.

**Here is the reason for generating invoice number:**

Quite a number of gateways including paypal require an invoice number be sent along with the payment request. Some gateways like Mollie require you to register the order with invoice number even before the payment is processed. So invoice number is kinda mandatory in those gateways.

**Features**

* Generate sequence invoice number for orders with status “CONFIRMED”.
* The default invoice number \(used by j2store\) would be used for all orders with the NEW status. You can treat these numbers as temporary numbers.
* The app also allows you to edit the invoice number and change it manually when required.
* Allows to define number zeros to be displayed after the invoice number.

**Installation**

1. Download the Invoice Prefix app generator from our site and install it using Joomla installer.
2. After installing the app, go to J2Store &gt; Apps and enable the app named Invoice Number Generator.
3. Once activated, click on open to configure the basic settings of the app.

**Configuration**

**Invoice prefix**

The prefix entered here will be used for the sequence invoice number generated.

**Number of leading zeros**

This option allows you to add zeros to be displayed after the invoice prefix and before the invoice number. If you have invoice prefix \(for example **INV-**\) and leading zeros as 4, then the invoice number would like **INV-0001, INV-2,…,INV-0010**. See the image below shows the leading zeros is set to 3 so the invoice numbers are **INVG-001, INVG-002**,..

![ipg01](https://raw.githubusercontent.com/j2store/doc-images/master/apps/Invoice-prefix-generator/ipg01.png)

![ipg02](https://raw.githubusercontent.com/j2store/doc-images/master/apps/Invoice-prefix-generator/ipg02.png)

**Automatically generate invoice number**

Choosing YES will generate the invoice number only when the order status matches the status selected below. See the image below.

**Generate an invoice number if the order has one of the selected statuses**

The invoice number will be generated only for the orders with the statuses selected here. For example, if you choose the status “Confirmed”, then the invoice number will be generated only for **Confirmed** order status. See the image below

![ipg03](https://raw.githubusercontent.com/j2store/doc-images/master/apps/Invoice-prefix-generator/ipg03.png)

**Allow editing invoice numbers manually**

Choosing this option YES will allow store owner to edit the invoice number by going to J2Store &gt; Sales &gt; Orders &gt; Edit order. For example sometimes you may need to change the invoice number for particular order status. In this case, you can use this option to edit the invoice number manually. See the image below

 

![ipg04](https://raw.githubusercontent.com/j2store/doc-images/master/apps/Invoice-prefix-generator/ipg04.png)

