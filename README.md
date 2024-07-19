
## Toy Store KPI Report 
Description: A Power BI KPI report for Maven Toys company, a toy store chain with multiple store locations in Mexico. This contains the transactional data from January 2022 - September 2023, along with information's about product and store locations.
Tables used: Inventory, Product, Sales, Store and Calendar (csv files)

## 𝐎𝐁𝐉𝐄𝐂𝐓𝐈𝐕𝐄 1: 𝐂𝐨𝐧𝐧𝐞𝐜𝐭 𝐚𝐧𝐝 𝐩𝐫𝐨𝐟𝐢𝐥𝐞 𝐭𝐡𝐞 𝐝𝐚𝐭𝐚.

To connect to the source data files, conduct basic profiling and QA tasks.
Tasks:
->Connect to the sales, products, stores, and calendar csv files.
->Review table columns, check for blank or null values, confirm that datatypes are accurately defined, and identify any primary and foreign keys.
->Take a moment to profile the data. How many transactions were recorded? How many stores does Maven Toys operate?
->Add calculated columns in the calendar table for ‘start of month’ and ‘start of week’.

## 𝐎𝐁𝐉𝐄𝐂𝐓𝐈𝐕𝐄 𝟐: 𝐂𝐫𝐞𝐚𝐭𝐞 𝐚 𝐑𝐞𝐥𝐚𝐭𝐢𝐨𝐧𝐚𝐥 𝐦𝐨𝐝𝐞𝐥.

To create relationships between fact and dimension tables, creating simple hierarchies, and adjusting model properties.
Tasks:
->Load the tables to the data model and create relationships from the sales table to the products, stores, and calendar tables.
->Your model should take the form of a star schema, with 1:many relationships between fact and dimension tables.
->Create a date hierarchy containing the ‘start of month’, ‘start of week’, and ‘date’ fields.
->Hide all foreign keys in the sales table from the report view.

## 𝐎𝐁𝐉𝐄𝐂𝐓𝐈𝐕𝐄 𝟑: 𝐀𝐝𝐝 𝐂𝐚𝐥𝐜𝐮𝐥𝐚𝐭𝐞𝐝 𝐦𝐞𝐚𝐬𝐮𝐫𝐞𝐬 𝐚𝐧𝐝 𝐅𝐢𝐞𝐥𝐝𝐬.

To enhance the data model and prepare for analysis by defining new measures and calculated fields.
Tasks:
->Create calculated columns in the sales table to pull in ‘cost’ and ‘price’ from the products table, then use those fields to calculate revenue and profit for each transaction.
->Create measures to calculate the count of orders (‘total orders’), sum of revenue (‘total revenue’) and sum of profit (‘total profit’).
->BONUS: Define new measures to calculate total revenue and profit without referencing the calculated columns in the sales table.

## 𝐎𝐁𝐉𝐄𝐂𝐓𝐈𝐕𝐄 𝟒: 𝐁𝐮𝐢𝐥𝐝 𝐚𝐧 𝐢𝐧𝐭𝐞𝐫𝐚𝐜𝐭𝐢𝐯𝐞 𝐫𝐞𝐩𝐨𝐫𝐭.

To visualize the data and create an interactive report to show orders, revenue and profit over time and by product category.
Tasks:
->Add KPI card visuals showing ‘total orders’, ‘total revenue’ and ‘total profit’ for the current month, along with monthly trends for each metric.
->Add a slicer to filter the report page by store location.
->Add a bar chart showing ‘total orders’ by product category, and a line chart showing ‘total revenue’ with the date hierarchy on the x-axis.
->Assemble the charts into a logical layout and adjust formatting, alignment and polish to finalize the report as you see fit.
