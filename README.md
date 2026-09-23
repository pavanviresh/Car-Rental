# Car-Rental
CAR RENTAL FLEET MANAGER
1. Project Description
The Car Rental Fleet Manager is a menu-driven Java console application designed to manage available vehicles, process customer bookings, handle vehicle returns, track maintenance schedules, and calculate total rental charges. The project focuses on practical applications of basic Java programming concepts, object management using arrays, and structured control flow statements.
2. Objective
The primary objective is to build an automated operational management system for a vehicle rental agency. The program allows administrators and staff to add new vehicles to the fleet, check availability, rent out cars, process returns with distance/day charges, schedule routine maintenance, and generate comprehensive fleet status reports.
3. Main Features
•	Add New Vehicles: Expand the agency fleet with vehicle model, registration number, daily rate, and vehicle type.
•	Rent Car: Check vehicle availability and rent out available cars to customers.
•	Return Car: Process returned vehicles, update availability, and calculate rental charges based on days and distance.
•	Maintenance Tracking: Mark vehicles for servicing or repair and update their operational readiness status.
•	View Fleet Status: Display a complete list of all cars with their current operational status and specs.
•	Interactive Console Interface: Menu-driven navigation allowing continuous operations until user selection of Exit.
4. Vehicle Categories & Pricing Structure
Vehicle Type	Base Rate / Day	Km Allowance	Extra Rate / Km
Sedan	₹2,500	200 km/day	₹12 / km
SUV	₹4,000	250 km/day	₹15 / km
Hatchback	₹1,800	150 km/day	₹10 / km
Luxury / Sports	₹7,500	300 km/day	₹25 / km

5. Program Flow
1. Start the program and initialize fleet data structures.
2. Display the main management control menu.
3. Prompt user for choice (Add, Rent, Return, Maintenance, View Fleet, Exit).
4. If Rent Car: Verify vehicle availability, calculate estimated cost, mark car as 'Rented'.
5. If Return Car: Input days used and distance covered, calculate final bill, set status back to 'Available'.
6. If Maintenance: Change status to 'In Service' or reset to 'Available' post-servicing.
7. Display transaction summary or bill breakdown.
8. Repeat program loop until user selects option 6 (Exit).
6. Control Statements Used
Control Statement	Purpose in the Project
if-else	Checks vehicle availability status (Available vs Rented/Maintenance) and calculates penalty charges.
switch	Handles top-level menu selection and vehicle category classification (Sedan, SUV, Hatchback, Luxury).
for loop	Iterates through the fleet array to display vehicle lists, calculate total revenue, and find matching IDs.
while / do-while	Keeps the application running repeatedly to manage continuous rental operations until Exit.
break	Terminates execution within switch cases and loop structures.

7. Java Concepts Demonstrated
•	Scanner class for standard console input and interactive prompts.
•	Variables & Data Types for storing rates, distances, vehicle status, and billing totals.
•	Arrays / Data Structures for managing lists of vehicle IDs, models, and availability states.
•	Arithmetic Operators for computing rental duration charges and extra kilometer penalties.
•	if-else conditional statements for status validation and discount/penalty logic.
•	switch-case statement for menu choice and vehicle type selection.
•	for loop for list traversal and fleet search.
•	do-while loop for persistent application execution.
8. Suggested Menu
===== CAR RENTAL FLEET MANAGER =====
1. View Fleet List
2. Add New Vehicle
3. Rent a Car
4. Return a Car
5. Maintenance Tracking
6. Exit
Enter your choice: 
9. Sample Working
Suppose the user rents an SUV (Base Rate ₹4,000/day, includes 250 km/day) for 3 days. Upon return, the customer has driven 850 km. The standard allowance for 3 days is 750 km (3 × 250 km). The excess distance covered is 100 km, charged at ₹15/km (₹1,500 extra). The total bill calculated is ₹12,000 (Base) + ₹1,500 (Extra km) = ₹13,500. The vehicle status is then automatically updated back from 'Rented' to 'Available'.
10. Sample Output
===== RENTAL BILL RECEIPT =====
Vehicle ID     : CAR-102 (Mahindra XUV700 - SUV)
Rental Duration: 3 Days
Distance Covered: 850 km (Allowed: 750 km)
------------------------------------
Base Rental Charges : ₹12,000
Extra Mileage Charges: ₹1,500 (100 km @ ₹15/km)
------------------------------------
TOTAL AMOUNT DUE    : ₹13,500
===== VEHICLE STATUS UPDATED TO AVAILABLE =====
11. Conclusion
The Car Rental Fleet Manager demonstrates how core Java programming structures—including switch-case statements, if-else conditional evaluations, for loops, and do-while loops—can be effectively integrated to build a practical, real-world fleet tracking and rental billing application. The modular menu-driven design ensures scalability for future enhancements such as database integration or object-oriented class expansion.
12. Reference to the Project Description
The project specifications require managing available cars, customer bookings, returns, and billing charges. It highlights specific control statements: if-else for checking vehicle availability, switch for vehicle category selection, for loop for iterating and displaying fleet records, and while/do-while loops for managing continuous operational options. The implementation faithfully fulfills all requirement criteria in a clean menu-driven console structure.
