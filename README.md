# Project
Excel Power Query Project Solution

Task 1: Import and append queries to combine sales data for the years 2020-2023.

1.	Open Excel and go to the "Data" tab.
2.	Click on "Get Data">" From File">" From Folder".
3.	Browse and select the folder that contains the sales data files you want to work with, then click on "OK".
4.	In the "Navigator" pane, select all the sales data files for the years 2020-2023 that you want to combine, then click on "Transform Data".
5.	In the Power Query Editor, Remove unwanted columns other than the name and content column.
6.	Click on the "Add Column" tab and select "Custom Column".
7.	Enter the following formula: “Excel.Workbook([Content])”.
8.	Click on "OK".
9.	Click on the expand button next to the custom column you just created.
10.	Select "Data" and click on "OK".
11.	And expand the “Custom.Data” column> click “OK”.

Task 2: Remove Duplicate or null Rows and columns to remove unwanted duplicate data.

1.	Remove the “Sr.no:” column due to repeated numbering, by selecting “Sr.no:” column>right-click>click on “remove column”.
2.	Select all columns> right-click on any column heading> click on ”remove duplicates”.
3.	Click on "Remove Rows" in the "Home" tab.
4.	Select "Remove Blank Rows" to remove any blank rows.
5.	Click on the "Remove Columns" dropdown in the "Home" tab and select "Remove Null Columns" to remove any null columns.

Task 3: Promote appropriate headers and assign appropriate data types to each column.

1.	Click on the "Transform" tab.
2.	Click on the "Use First Row as Headers" button.
3.	Each column will now have appropriate headers.
4.	Select the headers of every required column which are without the appropriate datatype.  
(Ex: Date and numerical columns)
5.	Right-click on the header> click on change > select the appropriate datatype.

Task 4: Use Replace Errors to correct errors in the data.

1.	Select all the columns.
2.	Go to the "Transform" tab in Excel Power Query.
3.	Click on "Replace Errors" from the “Replace values” dropdown menu.
4.	Enter “null” in the navigator box > click on “OK”.

Task 5: Use Fill Down to fill in missing data.

1.	Right-click on the column that has missing data.
2.	Select "Fill" from the right-click menu.
3.	Choose "Down" to fill in the missing values.
Task 6: Create a new index column with the column name “Sr.no".

1.	Click on the "Add Column" tab and select "Index Column".
2.	Select "From 1" as the starting value and "1" as the increment.
3.	Right-click on the index column and select "Rename". Enter "Sr.no" as the new column name.

Task 7: Import profit data and merge queries to combine the sales and profit data.

1.	Go to the "Home" tab in Power Query Editor.
2.	Click on the "New Source" dropdown menu.
3.	Select "File" from the dropdown menu.
4.	Choose the Excel file containing the profit data that you want to import.
5.	Select the sheet that contains the profit data.
6.	Click on "OK" to import the profit data into Power Query Editor.
7.	Then, click on the "Merge Queries" dropdown menu.
8.	Select "Merge Queries as New" from the dropdown menu.
9.	Select the sales data query and the profit data query.
10.	Select the "Sr.no" and “Order ID” columns in both queries as the common column to merge on.
11.	Click on "OK" to merge the queries.
12.	The merged query will show up as a new table with the combined sales and profit data. 
13.	Rename the new query to something like "Sales and Profit".


Task 8: Use date functions to analyse sales trends over time in each quarter of the year.

1.	Select the “Order date” column.
2.	Click on the "Add Column" dropdown in the "Add Column" tab> select "Date"> "Quarter"> “Quarter of the Year”.

Task 9: Create a conditional column to identify the Profit/loss status.

1.	Click on the "Add Column" dropdown in the "Add Column" tab and select "Conditional Column".
2.	Enter a name for the new column.
3.	In the "New Column" dialogue box, enter the following formula:
4.	= if [Profit] > 0 then "Profit" else "Loss"
5.	Click on "OK" to create the new column.
6.	Click on the "Close & Load" dropdown arrow in the "Home" tab. 
