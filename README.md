# Yelp-Analysis-Using-DataBricks
Large-scale Yelp business data pipeline using PySpark and Spark SQL on Databricks — 1M+ records cleaned, engineered, and analyzed for business insights.

### Dataset Overview
- 1,000,000 records loaded from Yelp Database sourced by Kaggle. Cleaned down to 738,000 valid USA businesses across 14 columns after removing nulls, invalid ratings, and non-US entries.

### Key Insights
##### Geographic Performance
- California dominates with 147,892 businesses and the highest average rating 
of 4.2, suggesting a strong and satisfied customer base. Arizona (3.95) and 
Hawaii (3.87) round out the top 3 states by rating quality. 

##### Category Performance
- Air Conditioning & Heating leads with a 3.99 avg rating (110K businesses)
- Plumbing follows at 3.93 (280K businesses)
- Delivery lags at 3.55 (347K businesses) — the largest category but lowest rate

##### Rating Distribution
- The majority of businesses are rated positively:
- 57.2% High (4.0+)
- 31.8% Medium (2.5–3.9)
- 11.0% Low (below 2.5)

##### Day of Week Trends
Friday (Day 5) and Thursday (Day 4) see the highest average ratings at 3.97 
and 3.95, while Tuesday (Day 2) has the lowest at 3.62. This suggests that 
customer satisfaction may vary by day of service.

##### More People, More Reviews 
California and New York carry the highest volume of low-rated businesses
(5,884 and 5,327 respectively), together accounting for nearly 14% of
all low-rated entries nationally. However, this is worth contextualizing —
both states also have the highest number of businesses and reviews overall,
which naturally leads to more low ratings.

##### Tools & Techniques Used
- PySpark for large-scale data ingestion, cleaning, and transformation
- Spark SQL for aggregations, window functions, and business analysis
- Databricks as the cloud compute and storage platform
- Dataset: 1M+ row Yelp business database
