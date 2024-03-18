### This project features an ETL pipeline, orchestrated by Airflow, designed to efficiently process data. The pipeline executes a sequence of operations starting with the retrieval of data from an AWS S3 bucket. It then employs Spark or Spark SQL to refine this data into a dataset that highlights orders with missing delivery deadlines. Finally, it uploads this cleansed dataset back into the designated folder within the same S3 bucket, ready for advanced analytical processing.

# Problem statement
In the evolving digital retail environment, retailers are navigating through significant changes. The rise of online retail giants has led to a noticeable shift in market dynamics, affecting traditional retail outlets adversely. Adopting an omni-channel retail strategy becomes imperative for survival and growth, particularly for those heavily invested in physical stores or with strong ties to traditional retail channels.

This data engineering initiative leverages a real-world retail dataset to scrutinize delivery efficiency on a large scale. The project aims to lay a robust groundwork for subsequent data analytics and modeling efforts and to generate daily summary reports for strategic decision-making.

The project involves a series of ETL tasks, utilizing Python, SQL, Airflow, and Spark, to construct pipelines that facilitate the downloading, processing, and uploading of data on AWS S3 for in-depth analytics.


# Dataset of choice
The dataset chosen for this endeavor originates from Olist, a Brazilian E-commerce firm, comprising multiple tables that provide a comprehensive view of their operations.


# Methodology
In this project, we've established an ETL pipeline with Airflow to manage data loading and scripting tasks within the S3 data lake. We scheduled the DAG to trigger the script execution on the EMR cluster, integrating job flow steps via the boto3 library, thus enabling the Spark job to run on a distributed cluster rather than a single local machine.



For access to the DAG script and additional support, please refer to the links below:

# for more details and help please refer to these following links:
https://github.com/ajupton/big-data-engineering-project

https://www.startdataengineering.com/post/how-to-submit-spark-jobs-to-emr-cluster-from-airflow/#commento-login-box-container

https://github.com/josephmachado/spark_submit_airflow
