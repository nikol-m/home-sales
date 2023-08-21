# Analyzing Home Sales Data with PySpark

#### Skills Used: PySpark, PysparkSQL, S3, Caching, Parquets
#### Data Source: https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.2/22-big-data/home_sales_revised.csv

## Overview
In this analysis, we leveraged PySpark and PySparkSQL to review home sales data. We also used caching and partitioning to determine which allowed for the fastest processing speed on this data. 

First, we created an instance of PySpark.SQL using `SparkSession` and read the file using `SparkFiles`.

Then we performed various queries on the dataset, including:
1. The average price of a four-bedroom house sold for each year.
2. The average price of a home for each year it was built that has three bedrooms and three bathrooms.
3. The average price of a home with three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet.
4. The average view rating for homes costing more than or equal to $350,000.

We ran the final query via PySparkSQL, via a cached table, and within a parquet dataframe to determine which was the fastest.

## Results & Conclusion
Based on this analysis, the fastest processing time was when we ran our query on the cached table with a speed of 0.2712 seconds.  


