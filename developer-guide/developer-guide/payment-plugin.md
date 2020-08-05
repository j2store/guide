# Payment plugin

* Introduction
* Plugin Structure
* Naming conventions
* The Manifest
* Creating the primary payment plugin class
* Display payment method in checkout
* Prepare to redirect to payment gateway or to process payment
* After payment is made

## Introduction <a id="introduction"></a>

Creating a payment plugin for J2Store is fairly a simple process if you are good in PHP and the Joomla MVC structure.

J2Store comes with a Payment library and wrappers that makes creating a plugin a breather. Integrations offered by different payment gateways can be broadly classified into two types

**1.Redirect \(also called Form, hosted, off-site\)** : Customer will be redirected to the payment gateway to make payment, like the Paypal standard. **2.Direct:** Customer will enter the credit card information in your site and stay in your site. Payment will be processed in the background using a cURL request.

So, before diving into the coding, you should first decide which type of integration are you going to make.

Most payment gateways provide both these types, while some gateways only provide you with a Redirect method.

## Plugin Structure <a id="plugin-structure"></a>

There is a folder structure and a few naming conventions, that should be followed during the development of a payment plugin for J2Store.

A typical payment plugin should look like this:

```text
├── plg_example/
│   ├── payment_example.php
│   ├── payment_example.xml
│   │   ├── payment_example/
│   │   ├── tmpl/
│   │   │   ├── form.php
│   │   │   ├── prepayment.php
│   │   │   ├── message.php
```

## Naming conventions <a id="naming-conventions"></a>

The manifest, the primary file, the template folder of the plugin should be start with the prefix ”**payment\_**”. Otherwise, J2Store will not recognise your plugin as a payment plugin. So our example plugin is named as: **payment\_example**

Make sure that the name of the file is in **lower case** and there are no spaces or any other characters in the file name.\#\#The Manifest

The plugin’s manifest should follow the joomla plugin creation basics.An example manifest should look like this:



```text
<?xml version="1.0" encoding="utf-8"?>
<extension version="2.5" type="plugin" group="j2store" method="upgrade">
    <name>Example</name>
    <version>1.0</version>
    <creationDate>June 2015</creationDate>
    <author>J2Store</author>
    <authorEmail>support@j2store.org</authorEmail>
    <authorUrl>http://www.j2store.org</authorUrl>
    <copyright>2015 Example Company</copyright>
    <license>GNU General Public License v3 or later versions</license>
    <description>Description of your plugin </description>
    
    <files>
        <filename plugin="payment_example">payment_example.php</filename>
        <filename>index.html</filename>
        <folder>payment_example</folder>     
    </files>
    <languages>
        <language tag="en-GB">languages/en-GB.plg_j2store_payment_example.ini</language>        
    </languages>
    <config>
    <fields name="params">
      <fieldset name="basic">

	<field 
	   name="articleid" 
	   type="text" 
	   size="10" 
	   default="" 
	   label="j2store_thanks_msg"
	   description="j2store_thanks_msg_desc"
	   />

	<field 
	   name="geozone_id" 
	   type="geozonelist" 
	   default="" 
	   label="J2STORE_GEOZONE" 
	   description="J2STORE_GEOZONE_DESC"
	   addfieldpath="/administrator/components/com_j2store/models/fields" 
	   />
        </fieldset>
    </fields>
</config>
</extension>
```

Also refer the manifest of the Paymill plugin that comes built in with the J2Store package.

The following parameters are standard in the payment plugins:

**articleid:** The ID of an article which should be displayed to the customer after the payment. Normally a thank you article.

**geozone\_id:** Store owner can restrict the appearance of this method to a particular geozone or for all geozones.

You can create more parameters depending upon your gateway requirements. Refer the plugins that come with the J2Store package.

## Creating the primary payment plugin class: payment\_example.php <a id="creating-the-primary-payment-plugin-class-payment_examplephp"></a>

The payment plugin class should essential have three methods :

1. \_renderForm\(\) - called at the Shipping and payment step
2. \_prePayment\(\) - called at the last checkout step
3. \_postPayment\(\) - called after the payment is made

Let us start creating the file.

Make sure the name of the class suffix is same as your plugin file’s name. And it should extend the J2StorePaymentPlugin class.

```text
defined('_JEXEC') or die('Restricted access');
require_once (JPATH_ADMINISTRATOR.'/components/com_j2store/library/plugins/payment.php');
class plgJ2StorePayment_example extends J2StorePaymentPlugin
{
	//IMPORTANT. The following variable identifies the plugin to j2store
	var $_element = 'payment_example';
```

As mentioned earlier, a payment plugin is triggered in three places in the Checkout steps \(for different purposes\). Let us go one by one based on their purpose.

**1.Shipping and Payment step**

The plugin will be listed in this step. When customer chooses your payment method, then you have the option to display a short message / instruction or a credit card form. The best use case is the display of a credit card form.

Use the following wrapper to display a form or a short message.

```text
  function _renderForm( $data )
{
    $html = $`this->_getLayout('form', $v`ars);    
    return $html;
}
```

The **\_getLayout method** will call the template / layout file \(form.php\) from the payment\_example/tmpl/ folder.

The **\_getLayout** method is actually a glorified include and it accepts a second argument, which can be an object or array. You can pass any data into the second argument which can be used in the form.php

The beauty of the \_getLayout method is that it will respect the template overrides. So users can override the layout without editing the core file.

**2.Prepare to redirect customer to the gateway or to process payment at the Order summary step \(Last step of the checkout\)**

When customer reaches this step, the order will be saved. And you will have an order id.

The following wrapper method is executed and it returns normally a **Place order button** \(may be a hidden form\). Check the Paymill plugin or the cash on delivery plugin.

```text
function _prePayment( $data )
{
	$vars = new stdClass();
	$vars->callback_url = JUri::root().'/index.php?option=com_j2store&view=checkout&task=confirmPayment&orderpayment_type=payment_example&paction=callback';
    $html = $this->_getLayout('prepayment', $vars);    
    return $html;
}
```

**3.After payment is made**

When customer clicks place order, they are either re-directed to the payment gateway or to the confirmPayment method in checkout \(controller\)

The confirmPayment method triggers the postPayment event \( which serves multiple purposes. For example, 1. Callback 2. To get a thank you article and display it to the customer\)

Here is a sample code for the \_postPayment wrapper

```text
function _postPayment( $data )
{
    // Process the payment
    $app = JFactory::getApplication();
    $paction = $app ->input->getString('paction');

    $vars = new JObject();

    switch ($paction)
    {
        case "display":
            $vars->message = 'Thank you for the order.';
            $html = $this->_getLayout('message', $vars);
            //get the thank you message from the article (ID) provided in the plugin params
            $html .= $this->_displayArticle();
            break;
        case "callback":
            //Its a call back. You can update the order based on the response from the payment gateway
            $vars->message = 'Some message to the gateway'
            $html = $this->_getLayout('message', $vars);
            echo $html; 
            $app->close();
            break;
        case "cancel":
            //cancel is called. 
            $vars->message = 'Sorry, you have cancelled the order'
            $html = $this->_getLayout('message', $vars);
            break;
        default:
            $vars->message = 'Seems an unknow request.'
            $html = $this->_getLayout('message', $vars);
            break;
    }

    return $html;
}
```

As you can see, we use a switch to serve different purposes.

In redirect methods, you will normally be asked to supply the following urls

```text
Return url : Where to return customers after payment is made
Cancel url : Where to return customers when they cancel
Callback (or notification): Where to send the callback (when payment is made)
```

For all these three, you can use the confirmPayment task \(in the checkouts.php controller\)

An example url would look like:

index.php?option=com_j2store&view=checkout&task=confirmPayment&orderpayment_type=payment\_example&paction=display

Notice the two parameters here:

```text
orderpayment_type = the name of the payment plugin
paction = an action to perform in the postPayment wrapper.
```

If you are integrating the direct \(credit card\) method, then refer the Paymill or the sagePay plugins in the j2store package for more information

A complete payment plugin class will look like the following

```text
loadLanguage('', JPATH_ADMINISTRATOR);
    }


    /**
     * Prepares variables for the payment form. 
     * Displayed when customer selects the method in Shipping and Payment step of Checkout
     *
     * @return unknown_type
     */
    function _renderForm($data)
    {
        $user = JFactory::getUser();
        $vars = new JObject();
        $vars->onselection_text = 'You have selected this method. You will be redirected.';
        //if this is a direct integration, the form layout should have the credit card form fields.
        $html = $this->_getLayout('form', $vars);

        return $html;
    }

    /**
     * Method to display a Place order button either to redirect the customer or process the credit card information.
     * @param $data     array       form post data
     * @return string   HTML to display
     */
    function _prePayment($data)
    {
        // get component params
        $params = J2Store::config();
        $currency = J2Store::currency();

        // prepare the payment form

        $vars = new JObject();
        $vars->order_id = $data['order_id'];
        $vars->orderpayment_id = $data['orderpayment_id'];

        F0FTable::addIncludePath(JPATH_ADMINISTRATOR . '/components/com_j2store/tables');
        $order = F0FTable::getInstance('Order', 'J2StoreTable')->getClone();
        $order->load(array('order_id' => $data['order_id']));
        $currency_values = $this->getCurrency($order);

        $vars->currency_code = $currency_values['currency_code'];
        $vars->orderpayment_amount = $currency->format($order->order_total, $currency_values['currency_code'], $currency_values['currency_value'], false);


        $return_url = $rootURL . JRoute::_("index.php?option=com_j2store&view=checkout&task=confirmPayment&orderpayment_type=" . $this->_element . "&paction=display");
        $cancel_url = $rootURL . JRoute::_("index.php?option=com_j2store&view=checkout&task=confirmPayment&orderpayment_type=" . $this->_element . "&paction=cancel");
        $callback_url = JURI::root() . "index.php?option=com_j2store&view=checkout&task=confirmPayment&orderpayment_type=" . $this->_element . "&paction=callback&tmpl=component";

        $orderinfo = $order->getOrderInformation();

        $vars->invoice = $order->getInvoiceNumber();

        $html = $this->_getLayout('prepayment', $vars);
        return $html;
    }

    /**
     * Processes the payment form
     * and returns HTML to be displayed to the user
     * generally with a success/failed message
     *
     * @param $data     array       form post data
     * @return string   HTML to display
     */
    function _postPayment($data)
    {
        // Process the payment
        $app = JFactory::getApplication();
        $paction = $app->input->getString('paction');

        $vars = new JObject();

        switch ($paction) {
            case "display":
                $vars->message = 'Thank you for the order.';
                $html = $this->_getLayout('message', $vars);
                //get the thank you message from the article (ID) provided in the plugin params
                $html .= $this->_displayArticle();
                break;
            case "callback":
                //Its a call back. You can update the order based on the response from the payment gateway
                $vars->message = 'Some message to the gateway'
                //process the response from the gateway
                $this->_processSale();
                $html = $this->_getLayout('message', $vars);
                echo $html;
                $app->close();
                break;
            case "cancel":
                //cancel is called. 
                $vars->message = 'Sorry, you have cancelled the order'
                $html = $this->_getLayout('message', $vars);
                break;
            default:
                $vars->message = 'Seems an unknow request.'
                $html = $this->_getLayout('message', $vars);
                break;
        }

        return $html;
    }


    /**
     * Processes the sale payment
     *	 
     */
    private function _processSale()
    {

        $app = JFactory::getApplication();
        $data = $app->input->getArray($_POST);

        //get the order id sent by the gateway. This may differ based on the API of your payment gateway
        $order_id = $data['YOUR_PAYMENT_GATEWAY_FIELD_HOLDING_ORDER_ID'];

        // load the orderpayment record and set some values
        $order = F0FTable::getInstance('Order', 'J2StoreTable')->getClone();

        if ($order->load(array('order_id' => $order_id))) {

            $order->add_history(JText::_('J2STORE_CALLBACK_RESPONSE_RECEIVED'));

            //run any checks you want here.
            //if payment successful, call : $order->payment_complete ();



            // save the data
            if (!$order->store()) {
                $errors[] = $order->getError();
            }
            //clear cart
            $order->empty_cart();
        }

        return count($errors) ? implode("\n", $errors) : '';
    }
```

If the payment is successful, you should call the following method

```text
$order->payment_complete();
$order->empty_cart();
```

If you want to update the status of order, you can call the following method

```text
$order->update_status($order_status_id, $notify_customer);
```

```text
$order_status_id = The status to which the order to be set.
You can get the ID of the order status from J2Store -> Localisation -> Order statuses.

$notify_customer = a Boolen value. Whether to notify the customer or not about the update to the order.
```

**Next steps**

Successfully created the payment gateway ? Well you can share it with other J2Store users via our Extensions Directory. Contact us to get your plugin listed for sale \(or for free distribution\).

