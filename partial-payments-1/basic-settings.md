# Basic Settings

## Enable partial payment <a id="enable-partial-payment"></a>

Three options are available as follows:No - If you would like to enable partial payment for specific product, set this option to NO. It will disable the partial payment mode globally. You should have to enable the partial payment at product level.Yes-optional partial payment - This allows partial payment mode as an option against normal full payment method.Yes-required partial payment - This makes partial payment as the only option.

* Select by defaultIf partial payment is to be set as the default payment mode, select it here.If not, you could choose the normal Full payment mode.
* Partial payment typeSelect if you wish to set up a fixed amount as the default amount to be paid or a plan or a % of the total amount.PlanThis option could be used to receive payments in installments as the name suggests.This type allows you to specify the description of the plan and split the payment in terms of percentage.Example:Pay in 2 installments/3 installments.You could also fix a duration for each payment, which is not possible for the rest of the two types.Example:Pay in 6 months/pay in 3 months.

## Percentage <a id="percentage"></a>

* This type lets you specify the percentage of amount that has to be paid by the user as a deopsit.
* The remaining amount has to be paid later.
* Example: Pay 50% of the amount as the initial deposit and then pay the remaining amount later on.

## Fixed Price <a id="fixed-price"></a>

* Using this method the exact amount that is to be paid as advance can be specified.
* The remaining amount could be collected later.
* Example:For a poduct whose total amount is,say 1000$, pay 250$ as the initial advance and the rest later.

Once the first part of the payment is collected,there will be an order scheduled for future payments at the backend.

* Amount/PlanThis option depends on the value chosen on the previous parameter.If you wish to collect a % of the total amount or a fixed amount the amount has to be specified here.If plan is chosen as the partial payment mode,the plan that has been created should be selected here.
* Order Status Scheduled order status for the future payments must be specified here.
* Cron URL The Cron URL should be mentioned here.

Cron URL can be used to run crons for scheduled payments.This could be used to send notifications to users and administrators that a payment due date is approaching.

Post running a cron, a Pay Now button would appear in the My Profile page under the Orders tab facilitating payment for users.

### Relevant Screenshot <a id="relevant-screenshot"></a>

![basic settings](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/basic-settings/app_partialpaymentbasicsettings.png)

## Mail Settings <a id="mail-settings"></a>

* Send email on enable payChoose Yes to send emails to the users when the payment due date approaches.
* Notify payment pending on
* Send reminder mails to customers through the days specified here after the payment date.
* Click Save.

### Relevant Screenshot <a id="relevant-screenshot-1"></a>

![mail settings](https://raw.githubusercontent.com/j2store/doc-images/master/partial-payments/basic-settings/app_partialpaymentmailsettings.png)

