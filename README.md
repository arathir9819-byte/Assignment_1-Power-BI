# Assignment_1-Power-BI
Data Transformation &amp; Data Modeling

  Imported the three files-List of Orders, Order Details, and Sales Target into Power BI and opened them in power Query.                                                                    
  Data Transformation:  Kept the first 500 rows from List of Orders, Changed Order Date to Date type, and Amount and Target to fixed Decimal Number., Changed Customer Name to Proper Case.                                                                                                                                                                              
  Then Merged State and City into a new column called Location([City] & "," & [State]).                                                                                                                                                               
 Created a Custom Column Profit Margin  (([Profit]/[Amount])*100) and a conditional column Profit Status as Loss if profit is Less then zero, Break-Even if zero, and Profit if greater then zero.
 
 Merging Data: Merged List of Orders and Order Details using Order ID to create a new column Orders Data.
 Removed the Duplicate Order IDs.
 
Sorting and Filtering : Sorted the Order Data by Order Date in descending order to see recent trends (Table.Sort(#"Removed duplicates", {{"Order Date", Order.Descending}}), and filtered it for Tamil Nadu for Regional analysis.

Grouping and Aggregating Data: Duplicated Order Details and found count of Order ID , average profit by Catetgory ,and total amount by Sub-category. Also duplicated Sales Target and found total target by month.

Data Modeling:  Created a relationship between List of Orders and Order Details using Order ID, and between Order Details and Sales Target using Category, and made sure the relationship is active.
