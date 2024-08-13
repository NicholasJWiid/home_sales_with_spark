# home_sales_with_spark

## Project overview
This project uses SparkSQL to determine key metrics about home sales data. Spark is also used to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Project requirements
1. Create a temporary table called home_sales and answer the following questions using SparkSQL:  
  * What is the average price for a four-bedroom house sold for each year? 
  * What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms?
  * What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet?
  * What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query.
2. Cache your temporary table home_sales.
3. Check if your temporary table is cached.
  * Using the cached data, run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000.
  * Determine the runtime and compare it to uncached runtime.
4. Partition by the "date_built" field on the formatted parquet home sales data.
5. Create a temporary table for the parquet data.
  * Run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000.
  * Determine the runtime and compare it to uncached runtime.
6. Uncache the home_sales temporary table.
7. Verify that the home_sales temporary table is uncached using PySpark.
