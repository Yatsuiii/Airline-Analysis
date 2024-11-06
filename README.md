# **Airline Dataset Analysis**

## **Project Overview**
We have a dataset consists of flight arrival and departure details for all commercial flights within the USA.
This is a large dataset: there are nearly 120 million records in total, and takes up 1.6 gigabytes of space compressed(bzip2) and 12 gigabytes when uncompressed(csv).
The goal of this project is to summarize the data by time periods, carriers,airports and understand different factors causing the airline delays.

## **Dataset**
This dataset can be find here [Airline on-time performance](http://stat-computing.org/dataexpo/2009/).
1. 1987-2009 (.bz2 format)
2. airports.csv
3. carriers.csv
4. plane-data.csv

## **Business Logic**
1. Are some time periods more prone to delays than others.
2. What are the best hours to travel.
3. Are some airports more prone to delays than others.
4. Are some carriers more prone to delays than others.
5. Do old planes suffer more delays.

## **Prerequisite Concepts**
1. Good understanding of Hadoop Environment.
2. Hive with Partitioning and Bucketing.
3. Tez/mapreduce framework.
4. Dimensional modeling for OLAP.
5. Splittable and non-splittable compression formats.
6. Different file formats(Avro, ORC, Parquet).
7. Data Driven Development for project building.

## **Datawarehouse Schema**

**Star Schema** is considered for data modeling because we are focused on analysing the data ie.. more read operations.

#### **Fact Table**

**data_fact_table** - records all the commercial flights arrival and departure details with delays.

#### **Dimension Table**

**airports_dim_table** - contains information about the airports.  
**carriers_dim_table** - contains information about the carriers.  
**plane_dim_table** - contains information about the planes.  


