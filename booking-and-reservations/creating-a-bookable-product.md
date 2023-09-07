# Creating a Bookable Product

Once the global settings have been completed, we are all set to create a bookable product. To create a bookable product, go to Article Manager and create a new article.

While creating new product, choose Booking as a product type.

Apart form the default options that are available for all the product types, these are the various parameters that distinguish the booking type product from the other product types:

* General tab
* Pricing tab
* Persons
* Availability

## General Tab <a href="#general-tab" id="general-tab"></a>

**Booking duration**

This options determines how long a booking is available. The duration can be defined by store admin (fixed block) or by customer (they need to input on the front-end). Duration can be set based on Hours, Minutes, Days or Months.

**Fixed blocks**

You can define a fixed block of dates that are to be allowed for booking while the others are being disabled in the frontend. For example: If you set up the booking duration parameter to be Fixed block of 1 day, then the user will be allowed to choose a single date for booking. That is, if customer books Dec 28, then the start date is Dec 28 and the End date is Dec 28.

![booking day](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/booking\_day.png)

* Fixed block of 1 Month - For example, if you are providing flats for a rent on monthly basis, you can choose the Booking duration Fixed block of 12 months

![booking month](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/booking-month-block.png)

On frontend, the blocks will be displayed like

![bookingmonth](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/booking-month.png)

* Fixed block of 3 hours - Take an example, a owner of conference hall allows hall booking for 3 hours. Lets see how you could setup the booking product for conference hall booking. Choose Fixed block of 3 hours as a booking duration.

![booking hour](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/booking-hour.png)

**Customer-defined blocks** You can allow the user to choose the start dates and end dates by themselves. You can also set up the minimum and maximum number of blocks that can be chosen when you choose the Booking duration as customer-defined blocks.

If you select the booking duration to Customer-defined blocks of 1 days, you would be prompted to choose the minimum and maximum duration allowed. If you choose 2 and 4 respectively, then the users will get a message if they choose dates that are more than 4 days or less than 2 days.

![booking duration](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/app\_bookingbookingdurationfixedback.png)

The frontend will be like this:

![booking duration front](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/app\_bookingbookingdurationfixedfront.png)

When the booking duration is chosen to be Customer-defined blocks of 1 days, the following options pop up:

* Minimum duration - To set the minimum number of blocks that have to be selected.
* Maximum duration - To set the maximum number of blocks that have to be selected.

The frontend will be like this:

![booking duration front1](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/app\_bookingbookingdurationcusfront1.png)

When the user chooses more blocks than the specified limit, error occurs as follows:

![booking duration front2](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/app\_bookingbookingdurationcusfront2.png)&#x20;

When the maximum duration is exceeded, the following error occurs:

![booking duration front3](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/app\_bookingbookingdurationcusfront3.png)

**Calendar display mode**

Choose when to display the calendar. You can choose to display the calendar by default or only after clicking.

The following video demonstrates the use of the calendar display mode option:

![calender review](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/app\_bookingcalendarviewbehav.gif)

**Allowing booking cancellation**

It is possible to choose whether the store admin want his/her user to have the option to cancel their booking. Setting YES to Can be cancelled? will allow customer to cancel the booking after it has been purchased.

## Pricing tab <a href="#pricing-tab" id="pricing-tab"></a>

The pricing tab for a booking type product has one extra option in addition to the default options as follows:

**Block pricing** While you are able to set a price to the product, the booking type product allows block-wise price charging in addition to the regular pricing which is now an added advantage.

Here is a screenshot to showcase the use of the block pricing option:

![booking pricing](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/app\_bookingpricingback.png) Now that we have set up block pricing, the users will be charged in this way:

![booking pricing front](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/app\_bookingpricingfront.png)

## Persons <a href="#persons" id="persons"></a>

This tab allows you to make the booking for multiple persons. To enable this feature, select YES. It is also possible to set a minimum and maximum number of persons.

For example, A car could be rented and maximum 4 persons can only travel. So if you set Minimum person : 1 and Maximum persons: 4, then booking will not be taken for more than 5 persons.

![booking persons](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/booking-enabe-persons.png)

![person count exceed](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/person-count-exceed.png)

**Persons will also come into the following cost options:**

Multiply block price by person count: If this option is enabled, all costs are multiplied by the number of persons the customer defines. It is also possible to enable person types. For example, Booking ticket for the journey might be having following restriction Only 2 Adults and 3 Children allowed. In this case, you could add person types and the pricing could be defined accordingly.

![booking person type](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/booking-person-types.png)

Once you enabled person types, you have the option to add multiple types.

Give your Person type a name (for example: Adult, Children) and define the cost (Base cost and Block cost) for the type. Adding a description is optional.

You can define a minimum and a maximum number for each person type. For example, you could require upto 2 adults and maximum 3 children for each booking. If you leave Max blank, there are no other restrictions than those of the bookable product itself.

![person type frontend](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/person-type-frontend.png)

## Availability <a href="#availability" id="availability"></a>

This tab controls the availability of blocks (i.e.) what blocks can be booked. Availability of blocks can be defined based on following time frame:

* Day(s)
* Month(s)
* Hour(s)
* Minute(s)

**Max bookings per block :** By using this option, you could define the number of bookings per block. For example, if you enter 2, more than 2 bookings on individual blocks are not allowed.

**Minimum block bookable and maximum block bookable :** If today is March 1 and you set minimum block bookable to 1 day into the future, then the first date a customer could book would be March 2. The same applies to the maximum date bookable. If you set maximum block bookable to 2 day into the future, then blocks avalaiable for booking are March 2, March 3.

**All dates are :** This option allows you to define specific date range to be availble or not available by default. The date range can be defined based on following time frames Months, Days, Hours, Minutes.

**Add date range**

To add a custom date range, click the Add Range button:

On the new row created, choose a range type, From / to range and choose whether it is bookable or not and a priority number. The following are the several date ranges:

* Date range – from and to will show a datepicker field
* Range of days – from and to will show a dropdown of days of the week (Monday to Sunday)
* Range of months – from and to will show a dropdown of months (January to December)
* Range of weeks – from and to will show a dropdown of weeks (1 to 52)
* Time ranges – from and to will show time inputs
* Date Range with time – a time range can be set based on a custom date range

For example, if you would like to make the days from March 20 to March 22 to be non bookable, then you will have to choose Available by default to the All dates option and the date range should be set like below:

![block available](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/block-available.png)

![non available dates](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/non-available-dates.png)

## More examples <a href="#more-examples" id="more-examples"></a>

### 1. Rent a car for a day <a href="#1-rent-a-car-for-a-day" id="1-rent-a-car-for-a-day"></a>

**Scenario:**

* Renting the car on a daily basis.
* Setting the capacity of car to 5 persons.
* Booking slots will be available only on week days and not on weekends.

**Creating a product**

* Go to Article manager and create a new article.
* Move to J2Store cart tab and choose YES to treat as a product.
* Choose product type as Booking and save.

**General tab** After creating the product, navigate to general tab.

**Booking duration** In our sample scenario, we are renting the car on a daily basis. So Set the Booking duration to Fixed blocks of 1 day(s).

![car rent](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/car-rent-general.png)

**Pricing** Set pricing for car renting and move to next tab.

**Persons** Our instance says that we are going to restrict the capacity only to 5 Persons. So following are the criteria to be set:

Min persons = 1 Max persons = 5

![car rent persons](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/car-rent-persons.png)

**Availablity** The car would be rented on a daily basis. The parameters should be set as follows:

Max bookings per block = 4

Minimum block bookable= 1 day(s) into the future Maximum block bookable= 30 day(s) into the future

To restrict the availability of the hall only to week days and block the availability on weekends:

Range type = Range of days Range = Saturday to Sunday Bookable = No

![car rent availablity](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/car-rent-availability.png)

Following is the screenshot of frontend:

&#x20;

![car rent front](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/car-rent-front.png)

**Video Tutorial:**

{% embed url="https://youtu.be/ZhnE1eLYO8s" %}



### 2. Renting the flats on monthly basis <a href="#2-renting-the-flats-on-monthly-basis" id="2-renting-the-flats-on-monthly-basis"></a>

**Scenario:**

* Renting the flats on a monthly basis.
* Multiple bookings per block cannot be allowed.

**Creating a product**

* Go to Article manager and create a new article.
* Move to J2Store cart tab and choose YES to treat as a product.
* Choose product type as Booking and save.

**General tab** After creating the product, navigate to general tab.

**Booking duration** In our sample scenario, we are renting the flats on a monthly basis. So Set the Booking duration to Fixed blocks of 12 month(s).

![house rent general](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/house-rent-general.png)

**Pricing**

Set pricing for car renting and move to next tab. There is no restriction for the capacity (persons) so navigate to the availability tab.

**Availability**

**Criteria**

* The flats would be rendted on monthly basis.
* Restrict multiple booking per block because multiple persons could not be booked for a single flat.

Max bookings per block = 1 Minimum block bookable= 1 month(s) into the future Maximum block bookable= 11 month(s) into the future

![house rent availablity](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/house-rent-availability.png)

**Screenshot of frontend**

&#x20;

![house rent frontend](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/house-rent-frontend.png)

**Video Tutorial:**

{% embed url="https://youtu.be/b_Gtt8G2xAQ" %}



### 3. Rent a sports helmet on hourly basis <a href="#3-rent-a-sports-helmet-on-hourly-basis" id="3-rent-a-sports-helmet-on-hourly-basis"></a>

**Scenario:**

* Bookings will be opened daily for hourly basis(say 3 hours).
* 10 bookings will only be taken per day.
* The availability time range is 12:00 am to 09:00 pm.

**Creating a product**

* Go to Article manager and create a new article.
* Move to J2Store cart tab and choose YES to treat as a product.
* Choose product type as Booking and save.

**General tab** After creating the product, navigate to general tab.

**Booking duration** Set this parameter to Fixed blocks of 3 Hour(s) to make the block available with custom time range.

![sports helmet general](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/sports-helmet-general.png)

**Pricing tab** Set the pricing accordingly and navigate to the availability tab.

**Availability tab** Max bookings per block = 10 Minimum block bookable = 0 days into the future Maximum block bookable = 1 month into the future Range type = Time range(all weeks) Range = 12:00 AM to 09:00 PM Bookable = Yes

![sports helemt availablity](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/sports-helmet-availability.png)

**Frontend screenshot**

&#x20;

![sports helemt front](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/sports-helmet-front.png)

**Video Tutorial:**

{% embed url="https://youtu.be/ZK9pXTPiOzM" %}



### 4. Tool kit rental in minutes: <a href="#4-tool-kit-rental-in-minutes" id="4-tool-kit-rental-in-minutes"></a>

**Scenario:**

* We are about to offer toolkit rental in terms of 90 minutes.
* Only 5 bookings would be possible per block(here let us suppose we have 5 tool kits).

**Creating the product:**

1. Go to article manager and create a new article.
2. Click on the J2Store cart tab and choose treat as product as Yes.
3. Set the product type as Booking and save.

**General Tab** Once the product type is chosen, navigate to the general tab.

**Booking duration:** The booking duration should be set to Fixed blocks of 90 minutes.

![Booking Minutes](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/Bookingminutes\_general.png)

&#x20;**Pricing tab:** Set the pricing accordingly and navigate to the availability tab.

**Availability tab:** Max bookings per block = 5 Minimum block bookable = 0 minutes into the future Maximum block bookable = 1 month(s) into the future

&#x20;

![booking minutes availablity](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/Bookingminutes\_availability.png)

**Frontend:**

&#x20;

![booking minutes frontend](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/creating-a-bookable-product/bookingmintes\_frontend.png)

**Video Tutorial:**

{% embed url="https://youtu.be/AfEe46mVujI" %}

