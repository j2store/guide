# Queue System

Starting from J2Store 3.2.20, we are supporting a queue system. The queue system, at the moment, is not used by the J2Store core functions.However a few apps are using it.

**Example:** The QuickBooks accounting integration, automated abandoned cart recovery email and so on. These apps are going to be released soon.

**Why we need a queue ?**

The J2Store core should not handle some of the mundane jobs during the runtime. For example, when a user registers at checkout, an “account created” email is being sent to the customer. J2Store waits for this email process to be completed before proceeding to the next step. Though it only takes a few seconds, this job should not be carried out by J2Store. All J2Store should do is add a queue job and go to the next one.The queue can be handled by the workers \(again J2Store but a separate section that does not affect the run time\) and processed.

**Why we need the cron ?**

Cron is present for a long time. But it had an internal, programmatic trigger. It is not really the optimal way of handling it.So we explicitly added a cron controller that fires an event along with a command. So in addition to j2store, the apps can also use it.Example: The queue worker can be triggered by the cron job \(Not necessarily by a user\)

**Another example:** We recently released a Subscriptions and memberships app. Now you can have recurring subscription products with auto-renewals and payments. The auto renewals are handled through a cron job.

