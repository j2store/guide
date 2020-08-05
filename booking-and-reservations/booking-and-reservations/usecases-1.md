# Usecases

In this guide we are going to get to know few scenarios where the booking extension could be used:

* Book a conference hall
* Book a service
* Book for a boat ride

## Book a hall <a id="book-a-hall"></a>

**Scenario:**

1. Renting the hall on a daily basis.
2. Setting the capacity of the hall to 50 persons.
3. Booking slots will be available only on week days and not on weekends.

**Creating a product**

1. Go to Article manager and create a new article.
2. Move to J2Store cart tab and choose YES to treat as a product.
3. Choose product type as Booking and save.

**General tab** After creating the product, navigate to general tab.

**Booking duration** In our sample scenario, we are renting the hall on a daily basis. So Set the Booking duration to Fixed blocks of 1 day\(s\).

**Pricing tab** Set the pricing and navigate to the next tab.

**Persons tab** Our instance says that we are going to restrict the capacity only to 50 Persons. So following are the criteria to be set:

Min persons = 1 Max persons = 50

**Availability tab** The hall would be rented on a daily basis. The parameters should be set as follows:

Max bookings per block = 1 Minimum block bookable= 1 day\(s\) into the future Maximum block bookable= 30 day\(s\) into the future

To restrict the availability of the hall only to week days and block the availability on weekends:

Range type = Range of days Range = Saturday to Sunday Bookable = No

Here are the screenshots that demonstrate the workflow of the above conditions:

![usecase1](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/booking-app-usecase1.png)

![usecase2](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/booking-app-usecase2.png)

![usecase3](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/booking-app-usecase3.png)

![useacse4](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/booking-app-usecase4.png)

## Service Booking <a id="service-booking"></a>

**Scenario:**

1. Bookings will be open daily for hourly basis\(say 3 hours\).
2. 10 bookings will only be taken per day.
3. The availability time range is 6:00 am to 11:00 pm.

**Creating a product**

1. Go to Article manager and create a new article.
2. Move to J2Store cart tab and choose YES to treat as a product.
3. Choose product type as Booking and save.

**General tab** After creating the product, navigate to general tab.

**Booking duration** Set this parameter to Fixed blocks of 3 Hour\(s\) to make the block available with custom time range.

![useacse5](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/booking-app-usecase5.png)

**Pricing tab** Set the pricing accordingly and navigate to the availabilitytab.

**Availability tab**

Max bookings per block = 10 Minimum block bookable = 0 days into the future Maximum block bookable = 1 month into the future Range type = Time range\(all weeks\) Range = 06:00 to 23:00 Bookable = Yes

![usecase7](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/booking-app-usecase7.png)

The above settings will implement the following changes in the frontend.

![usecase6](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/booking-app-usecase6.png)

![usecase8](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/booking-app-usecase8.png)

## Book for a boat ride <a id="book-for-a-boat-ride"></a>

**Instance** An owner of boat offers boat ride for daily on hourly basis. The duration of journey is 2 hours and the start times are 10:00 AM, 2:00 PM, & 6:00 PM. The booking price for Adults and Children can be vary. The maximum capacity of boat is 25.

**Configuration of bookable product**

1. Go to Article manager and create a new article.
2. Move to J2Store cart tab and choose YES to treat as a product.
3. Choose product type as Booking and save.

**General tab** After creating the product, navigate to general tab.

**Booking duration** In our example, the duration of boat ride is 2 hours. So set booking duration to Fixed blocks of 2 Hour\(s\).

**Persons tab** In this example, the pricing can be vary based on person types. To set different pricing for Adults and Children, Enable person types.

Set YES to Enable person types and click on Add person types button to add person type Adults and Children. And then define the base cost, block cost, minimum and maximum number for each person type.

Take a look at below demo screen shot to see how the parameters under person tab are configured.

![booking person](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/usecase3-booking-person.png)

**Availability**

Maximum bookings per block = 25 All dates are = not available by default

Add time range for boat ride by referring to the below picture

![booking availablity](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/usecase3-booking-availability.png)

**Frontend**

![booking frontend](https://raw.githubusercontent.com/j2store/doc-images/master/booking-and-reservations/usecases/usecase3-booking-frontend.png)

