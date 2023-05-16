# Home_Sales

Answering the following questions using SparkSQL:

  1- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

+----------+---------+
|date_built|avg_price|
+----------+---------+
|      2010|296800.75|
|      2011| 302141.9|
|      2012|298233.42|
|      2013|299999.39|
|      2014|299073.89|
|      2015|307908.86|
|      2016|296050.24|
|      2017|296576.69|
+----------+---------+

  2- What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
  
  +----------+---------+
|date_built|avg_price|
+----------+---------+
|      2010|280447.23|
|      2011|281413.45|
|      2012|295858.68|
|      2013|295142.13|
|      2014|294195.13|
|      2015|291788.36|
|      2016| 287812.6|
|      2017|282026.59|
+----------+---------+

  

  3- What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
  
  +----------+---------+
|date_built|avg_price|
+----------+---------+
|      2010|280447.23|
|      2011|281413.45|
|      2012|295858.68|
|      2013|295142.13|
|      2014|294195.13|
|      2015|291788.36|
|      2016| 287812.6|
|      2017|282026.59|
+----------+---------+


  4- What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
Cache your temporary table home_sales.

+----+---------+
|view|avg_price|
+----+---------+
|   0|403848.51|
|   1|401044.25|
|  10|401868.43|
| 100|1026669.5|
|  11|399548.12|
|  12|401501.32|
|  13|398917.98|
|  14|398570.03|
|  15| 404673.3|
|  16|399586.53|
|  17|398474.49|
|  18|399332.91|
|  19|398953.17|
|   2|397389.25|
|  20|399522.81|
|  21|399758.88|
|  22|402022.68|
|  23|403411.92|
|  24|400284.92|
|  25|401298.69|
+----+---------+



Check if your temporary table is cached.

Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

Partition by the "date_built" field on the formatted parquet home sales data.

Create a temporary table for the parquet data.

Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

Uncache the home_sales temporary table.

Verify that the home_sales temporary table is uncached using PySpark.
