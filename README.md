# Redfin Analytics Pipeline

## Overview
The "Redfin Analytics" project is an implementation of an Extract, Transform and Load (ETL) workflow using Apache Airflow. The goal is to extract real estate market data from Redfin, perform specific transformations and load the results into an Amazon S3 bucket. The data will then be transferred to Snowflake for data analysis and feeding into a BI dashboard.

## Transfer to Snowflake and Dashboard in BI
After loading the data into S3, the next step will involve transferring the data to Snowflake. Configure your Snowflake credentials in the config.py file and add tasks to the DAG to carry out the transfer.

Finally, using Business Intelligence (BI) tools such as Tableau, Power BI or Looker, you can create informative dashboards and visualizations from the data stored in Snowflake.


## Contributions
Feel free to contribute to this project! If you find problems or have suggestions for improvements, open an issue or send a pull request.
