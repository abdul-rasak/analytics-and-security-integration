# Analytics and Security Integration - My 2 Features
### Inventory Management Software - Group Assignment

> This document contains only my two independent features for the Analytics and Security Integration module. Both features are designed to be simple, practical, and distinct.

---

### FEATURE 1: ANALYTICS FOCUS

#### 1. Feature Title
Slow-Moving and Dead Stock Analytics

#### 2. Description
This feature helps identify products that are not selling or are selling very slowly. Instead of tracking best-sellers, it focuses on non-performing stock that is occupying warehouse space and tying up business capital. It helps managers decide what to put on discount, return to supplier, or discontinue.

#### 3. How the Feature Works
In the Inventory Management System:

1.  The system reviews sales history for every product, checking the last date it was sold and how frequently it sells.
2.  It automatically groups products into three categories:
    *   **Active Stock:** Sold within the last 30 days.
    *   **Slow-Moving Stock:** Not sold for 30 to 90 days.
    *   **Dead Stock:** Not sold for more than 90 days.
3.  On the manager's dashboard, it displays a list of slow-moving and dead stock items, showing the quantity on hand, the total monetary value locked, and the number of days since last sale.
4.  Managers can filter the results by category, warehouse, or supplier to find patterns.
5.  At the end of each month, the system generates a summary report to support decisions on promotions or stock clearance.

**Benefit:** Reduces storage costs and prevents money from being stuck in unsellable inventory.

---

### FEATURE 2: SECURITY FOCUS

#### 1. Feature Title
Sensitive Action Audit Trail with Anomaly Flagging

#### 2. Description
This feature is a security log that tracks all sensitive actions inside the inventory system. Sensitive actions include changing stock quantity manually, deleting a product, changing product price, and changing user permissions. If an unusual or risky pattern is detected, the system flags it for the administrator to review.

This ensures accountability and prevents internal fraud or mistakes.

#### 3. How the Feature Works
In the Inventory Management System:

1.  **Automatic Logging:** Whenever a sensitive action occurs, the system records:
    *   Who did it (User Name and Role)
    *   What was done (e.g., "Changed quantity of Item #102 from 50 to 5")
    *   When it was done (Date and Time)
    *   Where it was done (IP address)

2.  **Tamper-Proof Storage:** The audit logs are stored in a separate, read-only log area. Regular users and even inventory managers cannot edit or delete these logs. Only the System Administrator can view them.

3.  **Simple Anomaly Rules:** The system checks for suspicious patterns using simple rules:
    *   More than 10 sensitive adjustments by one user within 10 minutes.
    *   Deletion or major quantity changes done outside official work hours.
    *   A low-level staff account attempting a high-level action like deleting products.

4.  **Flag and Alert:** When a rule is triggered, the system does not stop the user, but it immediately marks that log entry as `FLAGGED` and sends a notification to the System Administrator.

5.  **Review Dashboard:** The administrator has a dedicated Audit Review page to see all logs, with flagged activities shown at the top for quick review.

**Benefit:** Provides accountability, discourages internal misuse, and creates evidence for security audits.# analytics-and-security-integration
Group 2 research and feature consolidation for the Analytics and Security integration module
