# Feature 1: Inventory Expiry Risk Prediction

### Description
This feature uses inventory data to identify products that are likely to expire before they are sold or used. It helps the business reduce product waste, avoid financial losses, and make better stock management decisions.

### How the Feature Works
The system monitors product expiry dates, current stock quantities, and past sales records. It compares the remaining shelf life of each product with its sales rate to identify items at risk of expiring.

When a product is likely to expire before being sold, the system generates an alert on the inventory dashboard. It can also suggest actions such as prioritising the product for sale, reducing its price, or limiting future purchases.

**Example:** If a store has 50 bottles of a product that will expire in 20 days, but usually sells only 10 bottles per month, the system flags the product as an expiry risk.

---

# Feature 2: Unusual Inventory Access Detection

### Description
This feature improves inventory security by identifying unusual activities performed by users within the system. It helps prevent unauthorised stock changes, suspicious transactions, and potential misuse of employee accounts.

### How the Feature Works
The system records user activities such as stock adjustments, product deletions, quantity changes, and login attempts. It monitors these activities and compares them with each user's normal access patterns and assigned permissions.

When an unusual activity is detected, the system generates a security alert for the administrator to review. For example, it may flag an employee who suddenly attempts to modify a large number of stock records or access restricted inventory information.

The administrator can investigate the activity, verify whether it was legitimate, and take appropriate action if necessary.

**Example:** If an employee who normally updates stock quantities for a few products suddenly attempts to change the quantities of 100 products within a short period, the system flags the activity for review. 
