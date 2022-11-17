# Big Data - Extract Transform Load - Amazon Shoppers Reviews

### Using PySpark, PgAdmin, and AWS' Relational Database in Google's Colab.


## Level1 - Objective

The purpose of this assignment was to use cloud ETL skills on big data from two of Amazon's available public datasets on product reviews. The goal is to perfrom the ETL process completely in the cloud and upload a DataFrame to an RDS instance.

This project required the use of Amazon Web Service (AWS), Relational Database Service (RDS), PostgreSql, Google Colab, and PySpark.

## Datasets
Two datasets were selected from Amazon's list of Reviews datasets at https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt:

`Video Games Reviews`
`Video DVD Reviews`

## AWS-RDS
Started by creating an AWS-RDS to connect to pgAdmin.

![AWS-RDS](images/RDS_videodb.png)

## Extracted the data from AWS-S3
![Extract_data](images/Extract_Data_fromS3.png)

## Transformed the data
![Transform_data](images/Transform_data.png)

## Loaded the Data
### Loaded the data from the dataframes to their respective tables in RDS using postgreSQL.
![Load_data](images/Loading_to_RDS.png)

Here is the data from review_id_table, products, customers, and vine_table from PostgreSQL.
![review_id_table](images/review_id_table_postgresql.png)
![products](images/products_table.png)
![customers](images/customers.png)
![vine_table](images/vine_table.png)

### Checking that the data load was successful in pgAdmin
![Sql_validation](images/sql_for_validating_data_load.png)


Similarly extracted, transformed and loaded the `video_DVD` review data from Amazon S3.