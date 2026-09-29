# Inventory Management Software: Analytics and Security Integration

**Module:** Analytics and Security Integration
**Proposal type:** Individual feature proposals (2 features)

---

## Feature 1: Smart Stock Trends Dashboard (Analytics)

### Description
The Smart Stock Trends Dashboard is a single screen that turns raw inventory records into easy-to-read charts and summaries. It shows which products sell fastest, which ones sit unsold on the shelf, and which ones are close to running out. Instead of scrolling through long tables of numbers, managers can see the health of their inventory at a glance.

### How the Feature Works
1. **Data collection:** Every time an item is added, sold, returned, or removed, the system already records it in the inventory database. This feature reads those records.
2. **Calculation:** The system totals up the sales of each product over a chosen period (for example, the last 7 days, 30 days, or 3 months). It then compares that total to the current stock level to estimate how many days the remaining stock will last.
3. **Display:** The results appear on the dashboard as:
   - A bar chart of the top 10 best-selling products.
   - A list of slow-moving products that have had little or no sales for a long time.
   - A "Running Low" panel that highlights items expected to run out soon.
4. **Filters:** Users can filter the dashboard by product category, date range, or warehouse location.
5. **Decision support:** A manager who sees that an item will run out in 5 days can reorder it early. A manager who sees an item that has not sold for 3 months can put it on discount instead of buying more.

**Benefit:** Fewer stock shortages, less money tied up in unsold items, and faster, data-based decisions.

---

## Feature 2: Role-Based Access Control with Activity Log (Security)

### Description
Role-Based Access Control (RBAC) makes sure that each person using the inventory system can only see and do what their job requires. Every user is given a role, and each role has a fixed set of permissions. The feature also keeps an activity log, which is a record of who did what and when, so any suspicious or accidental change can be traced.

### How the Feature Works
1. **Roles are defined:** The system has a small set of roles, for example:
   - **Admin:** Can manage users, change settings, and see everything.
   - **Manager:** Can view reports, approve orders, and edit stock records.
   - **Staff:** Can only add or update stock counts for their own assigned location.
   - **Viewer:** Can only look at stock levels and cannot change anything.
2. **Login and role check:** When a user logs in with their username and password, the system looks up their role. It then shows only the menus and buttons that role is allowed to use. For example, a Staff member will not see the "Delete Product" or "Manage Users" options.
3. **Permission check on every action:** Even if someone tries to reach a restricted page directly, the system checks their role again before allowing the action and shows an "Access Denied" message if they are not permitted.
4. **Activity log:** Each important action (logging in, changing a quantity, deleting a product, changing a price, or a failed login attempt) is saved with the username, the date and time, and a short description of what happened.
5. **Review:** Admins can open the activity log and search it by user, date, or type of action. If stock numbers suddenly look wrong, they can check the log to find out who changed them and when.

**Benefit:** Protects sensitive data from unauthorized changes, reduces mistakes and internal theft, and creates accountability for every change made in the system.

---

## Summary

| | Feature 1 | Feature 2 |
|---|---|---|
| **Title** | Smart Stock Trends Dashboard | Role-Based Access Control with Activity Log |
| **Focus** | Analytics | Security |
| **Main goal** | Help managers make better stock decisions using data | Protect data by limiting access and tracking changes |
| **Main users** | Managers and owners | Admins (with effects on all users) |
