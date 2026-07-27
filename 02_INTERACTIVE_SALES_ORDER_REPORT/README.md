# Interactive Sales Order Report

1.Project Overview
This project demonstrates an Interactive Classical Report developed in SAP ABAP using three custom database tables. The report displays sales order information in the basic list and provides detailed customer, product, and order information in the secondary list using the **AT LINE-SELECTION** event.

2. Objective
To develop an Interactive Classical Report that allows users to view sales order data and navigate to detailed information by double-clicking on a selected sales order.

3. Custom Tables Used
*ZCUSTOMER1 – Stores customer information.
* ZPRODUCT1 – Stores product information.
* ZSALES_ORDER – Stores sales order transactions.

4. Functional Requirements
* Selection Screen
- Select sales orders using **Order ID**.

* Basic List (Primary List)

Display the following fields:
- Order ID
- Customer Name
- City
- Product Name
- Quantity
- Product Price
- Total Amount (Quantity × Price)

The report retrieves data by joining all three custom tables.

* Interactive List (Secondary List)

- When the user double-clicks on a sales order, the report displays:

* Customer Details
- Customer ID
- Customer Name
- Mobile Number
- City

* Product Details
- Product ID
- Product Name
- Category
- Price

* Order Details
- Order ID
- Order Date
- Quantity
- Total Amount

5. SAP ABAP Concepts Used:
  
- Interactive Reporting
- SELECT-OPTIONS
- INNER JOIN
- Internal Tables
- Work Areas
- WRITE Statement
- HIDE Statement
- AT LINE-SELECTION Event
- TOP-OF-PAGE
- END-OF-PAGE
- Modularization (INCLUDE Programs)

6. Expected Output :

- Selection Screen
- Basic Sales Order List
- Interactive Detail Screen on Double Click

7. Learning Outcome :
This project demonstrates the implementation of SAP ABAP Interactive Reporting using classical events, data retrieval from multiple custom tables, and drill-down navigation through the **AT LINE-SELECTION** event.
