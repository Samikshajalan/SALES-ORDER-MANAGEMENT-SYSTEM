* Project Overview
This project demonstrates a Classical ALV Report developed in SAP ABAP using three custom database tables. The report displays sales order information in an ALV Grid by fetching data from customer, product, and sales order tables. It includes ALV features such as dynamic field catalog, zebra layout, sorting, optimized column width, calculated fields, and a customized report heading.
Objective. To develop a Classical ALV Report that enables users to retrieve and display sales order information in a structured ALV Grid with sorting, formatted layout, and a professional report header.

* Custom Tables Used
1.ZCUSTOMER1 – Stores customer information.
2.ZPRODUCT1 – Stores product information.
3.ZSALES_ORDER – Stores sales order transactions.

* Functional Requirements
Selection Screen

*The report allows users to filter records using:

Order ID (Select-Option)
Customer ID (Select-Option)
Checkbox Parameter
ALV Report

2.The report displays the following fields:
Order ID
Customer ID
City
Material ID
Material Name
Quantity
Product Price
Total Amount (Quantity × Price)

3. The report retrieves data by joining all three custom tables using INNER JOIN.

4. The Total Amount is calculated dynamically before displaying the ALV output.

5.Forms Used
GET
Retrieves data from custom tables.
Performs INNER JOIN between sales order, customer, and product tables.
Calculates Total Amount.
FIELDCATEGLOG
Creates the Dynamic Field Catalog.
Defines column names, sequence, and output length.
LAYOUT
Enables Zebra Pattern.
Optimizes column width automatically.
SORT
Sorts the ALV output by Order ID in ascending order.
EVENT
Registers ALV Events.
Calls the TOP_OF_PAGE event.
HEADING

6. Displays:
-Report Title
-Username
-Current Date
using REUSE_ALV_COMMENTARY_WRITE.

7. DISPLAY
Displays the report using REUSE_ALV_GRID_DISPLAY.

* SAP ABAP Concepts Used
Classical ALV Report
SELECT-OPTIONS
PARAMETERS
INNER JOIN
Internal Tables
Work Areas
Dynamic Field Catalog
Layout Customization
Zebra Pattern
Column Width Optimization
Sorting
ALV Events
TOP_OF_PAGE Event
Modularization (INCLUDE Programs)
REUSE_ALV_GRID_DISPLAY
REUSE_ALV_COMMENTARY_WRITE
Expected Output
Selection Screen
Classical ALV Grid Output
Report Heading (Title, Username, Date)
Sorted ALV Output
Zebra Pattern Layout
Calculated Total Amount

*Learning Outcome
This project demonstrates the implementation of a Classical ALV Report using SAP ABAP. It covers data retrieval from multiple custom tables through INNER JOIN, dynamic field catalog creation, ALV layout customization, event handling, sorting, calculated fields, and displaying a professional report header using standard ALV function modules.
