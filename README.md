# home-sales

# Analyzing Home Sales Data with PySpark

#### Skills Used: PySpark, PysparkSQL, S3, Caching, Parquets
#### Data Source: https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.2/22-big-data/home_sales_revised.csv

## Overview
For this analysis, I employed PySpark and PySparkSQL to delve into home sales data. I also harnessed caching and partitioning techniques to optimize processing speed for this dataset.

To begin, I initiated a PySpark.SQL instance using `SparkSession` and read the file utilizing `SparkFiles`.

Next, I executed several queries on the dataset, specifically focused on:
1. Calculating the average price of four-bedroom houses sold each year.
2. Determining the average price of homes for each year of construction, considering properties with three bedrooms and three bathrooms.
3. Finding the average price of homes featuring three bedrooms, three bathrooms, two floors, and a minimum of 2,000 square feet.
4. Evaluating the average view rating for homes priced at or above $350,000.

To assess performance, I executed the final query through PySparkSQL, utilizing a cached table and a parquet dataframe, comparing the processing speeds of each approach.

## Results & Conclusion
Upon analyzing the outcomes, I found that the most rapid processing time was achieved by running the query on the cached table, completing in just 0.2712 seconds.
