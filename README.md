# Real Estate Data Analytics ETL Project

## Overview
This project is a comprehensive Redfin Real Estate Data Analytics ETL (Extract, Transform, Load) pipeline using Python, Apache Airflow, Snowpipe, Snowflake, and AWS services. The goal is to connect to the Redfin data center, extract real estate data using Python, transform the data with Pandas, and load it into an Amazon S3 bucket. Both the raw and transformed data will be stored in separate Amazon S3 buckets.

Once the transformed data is available in the AWS S3 bucket, Snowpipe will be triggered automatically. Snowpipe will execute a COPY command to load the transformed data into a Snowflake data warehouse table. Finally, Power BI will be connected to the Snowflake data warehouse for visualization and insights.

Apache Airflow, an open-source platform for orchestrating and scheduling workflows, will be used to automate and manage the entire ETL process.

## Project Steps:

Source: Redfin data center
Extraction: Python script using pandas
Load: Raw data is stored in an Amazon S3 bucket
Transform: Data transformation using pandas
Load to Snowflake: Transformed data is loaded into a Snowflake data warehouse table
Visualization: PowerBI connected to the Snowflake data warehouse


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

## Setup Instructions:
Airflow Setup:

Ensure that Apache Airflow is installed on your EC2 instance.
Access Airflow on port 8080 (http://YOUR-IP-FROM-EC2:8080) with login credentials (admin/PASS-FROM-VISUAL-STUDIO-WHEN-YOU-START-AIRFLOW).
EC2 and VSCode Connection:

Use SSH to connect to the EC2 instance from VSCode.
Redfin Analytics DAG Execution:

Run the DAG in Apache Airflow to initiate the ETL process.
Data Download:

Download Redfin data from Redfin Data Center.
S3 Configuration:

Configure S3 buckets for receiving raw and transformed data.
Snowflake Setup:

Execute SQL queries to set up the Snowflake database, schema, and table.
Ensure AWS credentials are appropriately configured.
Snowpipe Configuration:

Set up a Snowpipe to automatically ingest data into Snowflake from the S3 bucket.
AWS SQS (Simple Queue Service):

Configure SQS for triggering Snowpipe through an SQS queue.
Visualization:

Connect PowerBI to the Snowflake data warehouse for visualization.

