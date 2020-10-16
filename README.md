# Project: Data Lake with Spark
This is an ETL, 'Extract, Transform, and Load', pipeline for the company Sparkify that extracts data from S3, transforms the data in Apache Spark into a set of fact and dimensional tables, and store the new data in another S3 bucket. This will give their analytics team the ability to easily find insights in what songs their users are listening to. This move from legacy Data Warehouse to a Data Lake will give the analytics team at Sparkify faster transformation of the data, and reduce the cost of operation.



## Files
The files used to make the etl, , and the warehouse are:
* etl.py
	* This file automates the extracting, transformation, and loading into the fact and dimension tables in the data lake.


## Prerequisites
* Apache Spark
* PySpark
* AWS IAM User
* AWS IAM Role
* AWS EMR with Spark
* AWS S3


## Launch
Run the etl.py file to load and insert into the new fact and dimension tables.

### Setting up the aws environment
create a s3 and set the key pair to
Spark-cluster-new-key-pair
start an EMR cluster
take the notebook and change to the new cluster
check that it runs
open an ssh with the correct address
ssh -i ~/.ssh/Spark-cluster-new-key-pair.pem hadoop@ec2-44-228-130-215.us-west-2.compute.amazonaws.com -ND 8157
run the EEEMMMRRRR thing with the correct cluster-id
aws emr ssh --cluster-id j-2MD2LOY3F7AO4 --key-pair-file ~/.ssh/Spark-cluster-new-key-pair.pem


## License

MIT License
