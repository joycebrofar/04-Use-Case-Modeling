# Problem 1

After reading the following narrative, perform the following: 

***a. Develop an activity diagram for each scenario.***  

***b. Complete a fully developed use case description for each scenario.*** 

Quality Building Supply has two kinds of customers: contractors and the general public. Sales of each are slightly different. 

A contractor buys materials by taking them to the checkout desk for contractors. The clerk enters the contractor’s name into the system. The system displays the contractor’s information, including current credit standing. The clerk then opens up a new ticket (sale) for the contractor. Next, the clerk scans in each item to be purchased. The system finds the price of the item and adds the item to the ticket. At the end of the purchase, the clerk indicates the end of the sale. The system compares the total amount against the contractor’s current credit limit and finalizes the sale if it is acceptable. The system creates an electronic ticket for the items, and the amount of the sale reduces the contractor’s credit limit. Some contractors like to keep a record of their purchase, so they request that ticket details be printed. Others aren’t interested in a printout. 

A sale to the general public is simply entered into the cash register, and a paper ticket is printed as the items are identified. Payment can be made by cash, check, or credit card. The clerk must enter the type of payment to ensure that the cash register balances at the end of the shift. For credit card payments, the system prints a credit card voucher that the customer must sign. 


# Problem 2

*Based on the following narrative, develop either an activity diagram or a fully developed description for the use case of ‘Add a new vehicle’ to an existing policy in a car insurance system. A customer calls a clerk at the insurance company and gives his policy number.* 

The clerk enters this information, and the system displays the basic insurance policy. The clerk then checks the information to ensure the premiums are current, and the policy is in force. 

The customer gives the make, model, year, and vehicle identification number (VIN) of the car to be added. The clerk enters this information, and the system ensures that the given data are valid. Next, the customer selects the types of coverage desired and the amount of each. The clerk enters the information, and the system records it and validates the requested amount against the policy limits. After all the coverages have been entered, the system ensures the total coverage against all other ranges, including other cars on the policy. Finally, the customer must identify all the drivers and the percentage of time they drive the car. If a new driver is then added, then another use case – ‘Add new driver’ – is invoked. 

At the end of the process, the system updates the policy, calculates a new premium amount, and prints the updated policy statement to be mailed to the policy owner. 


***A. Given the following list of classes and associations for the previous car insurance system, list the preconditions and postconditions for the use case ‘Add a new vehicle’ to an existing policy. Classes in the system include:*** 

- Policy 
- Insured Person 
- Insured Vehicle 
- Coverage 
- Standard Coverage (list standard insurance coverages with prices by rating category) 
- Standard Vehicle (list all types of vehicles ever made) 


Relationships in the system include: 
- The policy has Insured Person (one-to-many) 
- The policy has Insured Vehicle (one-to-many) 
- The vehicle has Coverages (one-to-many) 
- The coverage is a type of Standard Coverage 
- The vehicle is a Standard Vehicle


### Reference
Satzinger, J., Jackson, R., & Burd, S. (2015). Systems analysis and design in a changing world – Course Technology. USA: Cengage Learning. 
