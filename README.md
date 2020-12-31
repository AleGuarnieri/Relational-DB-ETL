# Relational Database ETL project

## Installation and execution
In order to run this project it is necessary to have installed python locally and to have the source datasets. 

First execute the file create_tables.py to prepare the database and the tables. 

After creating all the tables according to the designed data model, execute etl.py to extract the data from the source datasets 
and transform and insert them into the 5 final tables. 

## Motivation
The goal of this project is to build a data model following the star schema with 4 dimensions tables and 1 fact table to let an hypotetic analytics team 
perform data analysis. 
An ETL process was put in place in order to extract, transform and load the data from the surce datasets into the 5 final tables.

## Details
The source datasets are a subset of a public dataset available in public S3 of AWS "s3a://udacity-dend/". (datasets are not loaded in this repository)

## File Description 
create_tables.py: it creates the "sparkify" database used for creating the data model and performing the ETL process. it also call the sql_queries.py file to drop the tables if they exists in the database and to create them again, following the star schema descigned for this project.

sql_queries.py: it is used by create_tables to drop and create the tables of the data model

etl.py: it contains the functions necessary to extract, tranform and load the data from the source datasets to the 5 final tables of the star schema

## Acknowledgements
Udacity provided the course material necessary to implement the project