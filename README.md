# Final_Data_Engineer_Task
Covid 19 Analysis for January 2022


This Jupyter Notebook outlines a high-level architecture for processing and analyzing COVID-19 data from Johns Hopkins University. While the data ingestion step into PostgreSQL is not implemented here, the notebook demonstrates the following capabilities:

## Data Loading and Transformation:

1. Load CSV files from a specified directory.
2. Filter data based on a date range.
3. Perform basic data cleaning and transformation (e.g., converting data types, handling missing values).

## Exploratory Data Analysis:

1. Create a scatter plot to visualize the distribution of confirmed cases across the globe.
2. Identify the top 10 countries with the most confirmed cases in January 2022 and present them in a bar chart.
3. Analyze how a specific metric (e.g., confirmed cases) changes over time.
4. Calculate the correlation between two numerical columns (e.g., confirmed cases and deaths).


This is my proposed high level architecture for this project

![Screenshot 2024-03-06 at 8 18 27 AM](https://github.com/Beebbbyy/Final_Data_Engineer_Task/assets/66125895/3737d3af-abd3-4d3b-8ba8-c8b701c70c43)

- Data Source: CSV files are uploaded to an Amazon S3 bucket which is an object storage service offered by Amazon Web Services (AWS).
- Processing: The data is then processed using AWS Glue which is a serverless data preparation service.
- Data Storage: After processing, the data is stored in Amazon Redshift which is a data warehousing service.
- Data Visualization: Finally, the data can be visualized using Microsoft Power BI which is a business intelligence tool.
- “AWS Athena”  the data can also be queried using AWS Athena, which is an interactive query service for Amazon S3.
