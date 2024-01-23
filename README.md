# Real Estate Data Analytics ETL Project

## Overview
This project is a comprehensive Redfin Real Estate Data Analytics ETL (Extract, Transform, Load) pipeline using Python, Apache Airflow, Snowpipe, Snowflake, and AWS services. The goal is to connect to the Redfin data center, extract real estate data using Python, transform the data with Pandas, and load it into an Amazon S3 bucket. Both the raw and transformed data will be stored in separate Amazon S3 buckets.

Once the transformed data is available in the AWS S3 bucket, Snowpipe will be triggered automatically. Snowpipe will execute a COPY command to load the transformed data into a Snowflake data warehouse table. Finally, Power BI will be connected to the Snowflake data warehouse for visualization and insights.

Apache Airflow, an open-source platform for orchestrating and scheduling workflows, will be used to automate and manage the entire ETL process.

## Project Components
Data Extraction (Python):

Connects to the Redfin data center as a data source.
Extracts real estate data using Python.
Data Transformation (Pandas):

Utilizes Pandas for data transformation tasks.
Cleans and prepares the data for loading.
Data Loading (Amazon S3):

Loads the raw and transformed data into separate Amazon S3 buckets.
Snowflake Integration (Snowpipe):

Initiates Snowpipe to automatically run a COPY command and load transformed data into a Snowflake data warehouse table.
Visualization (Power BI):

Connects Power BI to the Snowflake data warehouse.
Creates visualizations and obtains insights from the data.
Workflow Orchestration (Apache Airflow):

Utilizes Apache Airflow to orchestrate and automate the end-to-end ETL process.
