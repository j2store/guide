# Table Rate Shipping

The table rate shipping plugin extends J2Store’s default standard shipping options giving you highly customizable shipping options.

Define multiple shipping rates based on location, price, weight, or item count.

* Add multiple shipping rules per shipping zone
* Several types of calculation method: Per order, per item, per class
* Add rules based on Weight, Number of items and price.
* Add costs per row, per item cost, a percentage and per weight unit

By using Table Rate Shipping it is possible for you to create complex rules for applying shipping cost.

You can define multiple rates based on the customer’s address, have multiple rates per zone, and add rules based on product weight, number of items, shipping class and price.

**Requirements**

* PHP version 5.4 and above
* J2Store 3.2.25 +
* Joomla 3.x

**Installation**

1. Download Table rate shipping plugin from our site and install it via Joomla installer.
2. After installing the package, go to J2Store &gt; Setup &gt; Shipping methods and enable Table Rate Shipping methods.
3. Once activated, open the plugin and start configuring shipping method.

**How the table rate shipping works** When a customer checks out items in their cart, the plugin looks at the customer’s destination \(geozone\) and then uses the table of rates you created to calculate total shipping. Each geozone can have its own rules, or multiple sets of rules, based on your shipping requirements.

You have to create shipping zones and its rules for calculating the shipping correctly.

**Configuration**

**Plugin settings** Before start creating shipping method, you will have to select the weight unit globally. Handling cost is optional.

![basic settings](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/tablerate-basicsettings.png)

**Creating Shipping method** Navigate to Shipping rule tab and start creating shipping method by clicking on the button Add shipping button.

![addshipmethod](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/tablerate-addshipmethod.png)

**Method title** Give the name of your shipping method. For example: Table rate

**Geo Zone** You can assign the shipping method to multiple zones. So that the shipping cost will be calculated by checking customer’s destination address.

**User group** Do you have different price for different customers ? And also wants to define the shipping cost for different customers ? Its also possible with this advance shipping plugin. The shipping method can be assigned to single or multiple usre group so that the shipping cost will be applied to the customer who is associated with the user group selected here.

**Shipping tax** If you would like to include tax to the shipping tax, you will have to select the tax profile here.

**Maximum shipping cost** You can assign a maximum shipping cost to a method. For example, if the shipping total calculated is greater than the maximum cost, the price is decreased to maximum cost amount.

**Calculation type** - Here you can decide how the plugin should calculate the shipping cost. The plugin provides three types of calculation methods:

* Per orderThis type of calculation method calculates the shipping cost for the entire cart. If there are multiple shipping costs in the cart, the class with the highest priority will be used. These can be set in the plugin that appears underneath the rate table when per order is selected.
* Per itemThis type calculates the shipping cost by checking each item in the cart with the rates defined in the plugin.
* Ship classEach shipping class in your cart is totaled and offered at a final rate.

**Handling cost per item** Apply a additional fee to the shipping cost calculated per item or per order or shipping class.

**Minimum cost per item** Set a minimum cost to the calculated item. The item calculated could be an individual item or shipping class based on above settings.

**Maximum cost per item** Set a maximum cost to the calculated item. The item calculated could be an individual item or shipping class based on above settings.

![shippingmethod](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/tablerate-shippingmethod.png) **Creating shipping rule** After filling all the fields on shipping method, click save and you will be asking to create shipping rule for the shipping method you created.

Click on Add Rule button to create shipping rule.

![shippingrule](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/tablerate-shippingrule.png)

**Shipping class** - If you would like to calculate the shipping based on shipping class, then you will have to select the shipping class here. If you don’t want to use shipping class, select No class.

**Condition** - This parameter allows customer to decide what product information the plugin should use to calculate shipping rates. Your options are:

1. Price – the price of the items
2. Weight – the weight of the items
3. Item Count – the number of an individual item

**Min-Max** The minimum and maximum range should be given here for the chosen condition. For example, if you have chosen Item count as a condition, then you have to give the quantity range using these parameters.

**Break** This option is used to stop calculating further shipping rates if you reach this row of the table.

**Abort** Enable this option to disable all rates or the shipping you are editing if the row you are editing matches any item/class being quoted.

**Row cost** This is the base cost for shipping. This cost will be added to the shipping cost.

**Weight cost** Enter the cost per weight unit for the products.

**Percentage \(%\) cost** The percentage of the products total should used to calculate shipping.

 **Shipping class** Shipping classes are used to restrict shipping by products. For example, you may have a product that weighs very large and needs special shipping price. In this case, you can use shipping class and create a shipping rule for that specific product. Multiple shipping classes can be created here. For example, special, normal, store pickup.

![createshiprules](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/tablerate-shiprulecreate.png)

You can create tables of rates that apply to different shipping classes. This gives you considerable flexibility when creating shipping methods.

 After creating shipping class, you will have to associate this shipping class to the product which needs special shipping charge.

![shipclass](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/tablerate-shipclass.png)

![prodship](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/tablerate-prodshipclass.png)

**Examples** Lets see some of the working examples below:

**1. Create a shipping method with shipping class** Consider a store owner is selling Teddy bear. His customer often buy multiple quantities of teddy bears. He wants to charge shipping cost of $4 and also would like to charge $2 for each teddy bear. Lets see how to create shipping rules for this scenario:

1. Create a geozone. If you wants to apply a shipping charge to the customers only from United States, then you will have to create a geozone for the country United States.
2. Then, go inside the plugin and create a shipping method.
3. Give a name for your shipping method and choose the geozone and user group.
4. Choose Ship Class as your calculation type and save. \(Note: You should have to create shipping class under the tab Shipping class\).
5. Now create the shipping rule like belowChoose your shipping class. For example, Sample.Condition - Item countMin-Max - 1 to 100Item cost - $2Row cost - $4

See the table below :

![ex1](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/tablerate-ex-1.png)

When customer purchasing cap, they will be charged like below

1 Teddy bear : $6 2 Teddy bears : $8 3 Teddy bears : $10

**2. Applying multiple rules to the same shipping class** Consider the store owner would like to apply shipping with on the basis of item’s quantity. For example, when people buy more than 2 teddy bears, then the shipping charge should be $16. So the original rate should be edited to a Minimum of 1 and maximum of 2 and then add the following shipping rule:

1. Choose shipping class. For example, Special
2. Condition - Item count
3. Min : 3 and Max : 1000
4. Item cost - $2
5. Row cost - $16

The table setup should be like below:

![ex2](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/tablerate-ex-2.png)

When customers purchase Teddy bears, they will be charged like below:

* > 2 teddy bears costs $8 for shipping \(2\*2\)+4
* > 3 teddy bears costs $22 for shipping \(3\*2\)+16

**3. Calculating shipping cost by weight** The shop owner decided to charge for a shipping based on weight. It’s more cost efficient for him to ship by weight, so he plans to re-structure his shipping rates like below:

0-0.5kg: $3.75 0.5-1kg: $5.30 1kg-2kg: $9.50

In this case, we are going to calculate the shipping based on the weight of the entire order so choose Per Order as the calculation type. He needs to create three rows, one for each rule he wishes to create. These will apply to any shipping class, with the weight condition, and a minimum and maximum weight applied.

**Use cases**

**1. Shipping products based on Geozone** Consider that store owner would like to ship some of his products to Mumbai and some products to Delhi. Configuring this type of shipping cost could be achieved by using Shipping class.

**Here is the scenario:**

1. Product A will be shipped from Mumbai
2. From Delhi warehouse, Product B should be shipped
3. If customer adds both product A and B to cart so shipping charge of both should be summed and shown up because Product A ship from Mumbai and B from Delhi so user have to pay two shipping cost.

Let me explain how to configure the table rate shipping based on above scenario.

**Step-1: Create geozone** Since the products are going to be shipped from different places, the geozones have to be created separately.

The below screenshot shows that we have created two geozones “Mumbai” and “Delhi”.

![usecase](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-1a.png)

**Step-2 Creating shipping class**

Since the shipping cost has to be calculated based on shipping class, there are two shipping classes needs to be created. We have created below two shipping classes

1. Mumbai
2. Delhi

![trusecase](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-1c.png) Then, assign the shipping class to the products accordingly.

**Cap** - We considered that this product will be shipped from Mumbai. So we assigned the shipping class “Mumbai” to this product. If you edit the product and navigate to J2Store Cart tab &gt; Apps tab, you would see the shipping class associated.

![usecase1d](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-1d.png)

**T-shirt** - and considered this will be shipped from Delhi so we assigned the shipping class “Delhi” to this product.

**Step-3: Creating shipping methods**

We have created two shipping methods using table rate shipping plugin.

1. Shipping cost 1 - This is to apply the shipping charge for the products to be shipped from Mumbai.
2. Shipping cost 2 - This is to apply the shipping charge for the products to be shipped from Delhi.

Now open the table rate shipping plugin and create the shipping method for Mumbai called “Shipping cost 1”. Assign the geozone “Mumbai”. Finally create the shipping rule using the shipping class.

The shipping cost 2 has been created similar to the shipping cost 1.

![usecaseb](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-1b.png)

**Frontend screenshots:**

Shipping charge applies when adding product A: 

![usecasee](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-1e.png)

Shipping charge applies when adding product B

 When adding both products, the shipping cost calculated by adding both charge:

![usecasef](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-1f.png)

![usecaseg](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-1g.png)

**2. Applying shipping charge based on location and quantity.** Consider that store owner would like to set the different shipping cost for Germany and France based on both order quantity and item quantity. Let’s see the scenario below:

**Scenario**

1. For customers from Germany,TOTAL of all Items from 1 to 12 = Flat shipping rate 7.20€TOTAL of all Items from 13 to xxx = shipping rate per Item 0.60 €That means,total of all Items =1 then the Shippng rate is 7.20 €total of all Items =12 then the Shippng rate is 7.20 €total of all Items =13 then the Shippng rate is 7.80 €total of all Items =30 then the Shippng rate is 18.00 €
2. For customers from France,TOTAL of all Items from 1 to 12 = Flat shipping rate 12.00€TOTAL of all Items from 13 to xxx = shipping rate per Item 1.00 €That means,total of all Items =1 then the Shippng rate is 12.00 €total of all Items =12 then the Shippng rate is 12.00 €total of all Items =13 then the Shippng rate is 13.00 €total of all Items =30 then the Shippng rate is 30.00 €

Here are the steps to configure the table rate shipping according to above scenario:

**Step-1 Creating geozones**

Since the shipping cost are going to be calculated based on Germany and France, you will have to create two different geozones.

![usecase2a](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-2a.png)

**Step-2 Creating a shipping method for scenario 1**

1. Create a shipping method and give the name to it. For example, we named it as “Shipping cost 1”
2. Then, choose Germany to the Geozone and select the usergroups.
3. Choose Per Order as a Calculation type and save.
4. Click on Add rules button to add shipping rules to the shipping method. Since the shipping cost will be different based on order quantity and item quantity, you will have to create two shipping rules.Here is how the shipping rule has to created:Shipping rule 1:Shipping class - Any classCondition - Item countMin - Max - 1 to 12Row cost - 7.2Shipping rule 2:Shipping class - Any classCondition - Item countMin - Max - 13 to 999Item cost - 0.6

Finally save.

![usecase2b](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-2b.png)

![useacse2d](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-2d.png)

![usecase2e](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-2e.png) **Step-3 Creating a shipping method for scenario 2**

Similar to the above step, create a shipping method. Then, choose France to the geozone and save.

Now create two shipping rules for this method as per below:

**Shipping rule 1:** Shipping class - Any classCondition - Item countMin - Max - 1 to 12Row cost - 12

**Shipping rule 2:** Shipping class - Any classCondition - Item countMin - Max - 13 to 999Item cost - 1

![usecase2c](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-2c.png)

![usecasef](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-2f.png)

![usecase2g](https://raw.githubusercontent.com/j2store/doc-images/master/shipping-methods/table-rate-shipping/table-rate-usecase-2g.png)

