# How Tax is Calculated:

## How Tax is Calculated:

### **Criteria based on which the tax calculations are done:**

  
**1. The country and region chosen by the user.** For example, if you have set up tax for the USA Geozones comprising all the US states, then users who choose this Geozone would only be levied tax.

  
**2. Address associated in the tax profile and Tax configuration:** The associated address chosen on the tax profile should match the option chosen for "Tax calculated based" on in the J2Store config.                       For example: If you choose the Shipping address in tax profile, then that should be chosen on the Tax config as well.

  
**3. Product should have tax profile associated with it:** You might want to associate the appropriate tax profile to the product. If not, that particular product would not have tax if its available on the cart.

  
So, when a user adds a product to the cart on the storefront, the address chosen should be having a tax rate set up, the product should have a tax profile associated to it and the Associated address should match the address chosen in the Tax config as well.  
If not, there might be conflicts on tax calculations.If you have any further queries on tax-related issues, do drop a support request to us or raise a ticket via the priority ticket system.

