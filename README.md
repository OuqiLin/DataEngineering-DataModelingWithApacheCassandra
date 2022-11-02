# DataEngineering-DataModelingWithApacheCassandra

## Overview
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in **understanding what songs users are listening to.**  
In this projects, we create an Apache Cassandra database and build up an ETL pipeline which can create queries on song play data to answer the questions. The ETL pipeline transfers data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables.  

## Datasets
A set of csv files named `event_data`, partitioned by date. Example of filepath of the csv files:
```
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
```
We will process these files into one single denormalized dataset (csv file) named `event_datafile_new.csv`.  
After creating this denormalized dataset, we load the data into tables in Apache Cassandra and run the target queries.  
