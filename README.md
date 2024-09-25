# Problem 1

### Contractor Sale Activity Diagram
![Contractor Sale Activity Diagram](https://github.com/joycebrofar/04-Use-Case-Modeling/blob/main/Contractor%20Sale%20activity%20diagram.drawio.png)

**Use Case 1: Contractor Purchase**

| Name | Description |
| ----------- | ----------- |
| Use Case Name | Contractor Purchase |
| Actors | Contractor, Clerk, System |
| Preconditions | Contractor must have an account with a credit limit |
| Postconditions | Sale finalized, electronic ticket created, credit limit updated |
| Main Flow | 1. Contractor selects items for purchase. |
|| 2. Contractor approaches the checkout desk for contractors.
|| 3. Clerk enters contractor’s name in the system.
|| 4. System displays contractor information, including credit status.
|| 5. Clerk opens a new sale ticket.
|| 6. Clerk scans the items.
|| 7. System retrieves prices and updates the ticket.
|| 8. Clerk finalizes the sale.
|| 9. System checks the total against the credit limit.
|| - If sufficient, sale is completed, and credit limit is reduced.
|| - If insufficient, the clerk is notified.
|| 10. If requested, the ticket details are printed. |


### General Public Purchase Activity Diagram
![General Public Purchase](https://github.com/joycebrofar/04-Use-Case-Modeling/blob/main/General%20public%20purchase.drawio.png)

**Use Case 2: General Public Purchase**

## Use Case Name: Create a new sale

| **Scenario**           | A new cash sale                                                                                                                                       |
|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Triggering Event**    | Cash customer wants to purchase items.                                                                                                               |
| **Brief Description**   | A cash customer wants to purchase items. The clerk enters the item ID, and the system creates a sales ticket. Customer pays with cash, check, or credit card. |
| **Actors**              | Sales clerk                                                                                                                                           |
| **Stakeholders**        | Sales clerk, Accounting department, Sales department                                                                                                  |
| **Preconditions**       | Inventory items must exist                                                                                                                            |
| **Postconditions**      | New sale is created. Sales line items are created and connected to the sale. Payment transaction is created.                                            |

### Flow of Activities

| **Actor**                                  | **System**                                                                                   |
|--------------------------------------------|----------------------------------------------------------------------------------------------|
| 1. Clerk starts new cash sale.             | 2.1 System finds item in inventory, finds price, displays information, adds to total.         |
| 2. Clerk enters each item.                 |                                                                                              |
| 3. Clerk indicates the end of the sale.    | 3.1 System calculates total.                                                                 |
| 4. Clerk indicates type of payment and enters information. | 4.1 System processes payment and creates payment transaction. |

### Exception Conditions

| **Actor**                                  | **System**                                                                                   |
|--------------------------------------------|----------------------------------------------------------------------------------------------|
| 2.1 If system has information missing, sales clerk calls manager and manually enters information. | |
| 4.1 If customer credit card fails approval, require cash or cancel sale.                       | |


# Problem 2

**Preconditions**

1. Valid Customer Identification: The customer must have a valid policy number that is recognized by the system.

2. Active Policy: The insurance policy linked to the policy number must be currently active and not lapsed.

3. Current Premiums: The premiums associated with the policy must be current, indicating that there are no outstanding payments that could affect the policy's validity.

4. Clerk Access: The clerk must have the necessary access to the system to view and update policy information.

5. Valid Input Data: The customer must be prepared to provide valid information regarding the new vehicle, including make, model, year, and VIN.


**Postconditions**
1. Vehicle Added: The new vehicle is successfully added to the existing policy, and its details are recorded in the system.

2. Coverage Information Updated: The selected types of coverage for the new vehicle are recorded and validated against policy limits.

3. Premium Calculated: The system recalculates the premium amount for the policy considering the addition of the new vehicle and its coverages.

4. Policy Updated: The insurance policy is updated to reflect the addition of the new vehicle and any changes in coverage.

5. Updated Policy Statement: An updated policy statement is generated and prepared for mailing to the policy owner, indicating the new details of the policy including the added vehicle and any adjustments in premium.

6. Driver Information Recorded: If new drivers are identified, their information is recorded, and if they are new to the policy, the use case "Add new driver" is invoked.


**The activity diagram should include the following steps:**
1. Clerk enters policy number.

2. System retrieves policy information.

3. Clerk verifies policy status and coverage capacity.

4. Clerk enters vehicle information (make, model, year, VIN).

5. System validates vehicle information.

6. Clerk selects coverages and amounts.

7. System validates coverage selections and amounts.

8. System checks coverage limits and other vehicles on the policy.

9. Clerk enters driver information.

10. System adds new driver (if necessary, invoking the "Add New Driver" use case).

11. System updates policy with new vehicle and driver information.

12. System calculates new premium.

13. System generates updated policy statement.


![P2 Activity Diagram](https://github.com/joycebrofar/04-Use-Case-Modeling/blob/main/P2%20Activity%20diagram.png)

## References

- Bors, M. L. (2018, April 15). Preconditions and Postconditions - Mátyás Lancelot Bors - Medium. Medium. https://medium.com/@mlbors/preconditions-and-postconditions-5913fc0fcdaf Indeed Editorial Team (Ed.). (2024, August 16). What Is a Use Case? (With Key Elements and an Example).
- Indeed. https://www.indeed.com/career-advice/career-development/use-case
- Lallie, H. S., Debattista, K., & Bal, J. (2020). A review of attack graph and attack tree visual syntax in cyber security. Computer Science Review, 35, 100219. https://doi.org/10.1016/j.cosrev.2019.100219
