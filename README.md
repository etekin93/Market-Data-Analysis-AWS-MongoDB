# Market-Data-Analysis-AWS-MongoDB
In this Project;
-Created Amazon VPC with 10.0.0.0/16 CIDR block. To be able process disaster recovery, distributed VPC over 4 different availability zones. Created Public Subnets with 10.0….0/24 CIDR blocks. Created route table and added subnets to this route table and, created internet gateway and attached it to VPC. Deployed EC2 in a public subnet and, installed MongoDB server inside of EC2.
-Pulled real time stock prices data from website into csv files. Migrated this csv files under one collection and converted to json documents in a MongoDB database by using Studio3t (client tool for MongoDB server). Exported json documents by using Studio3t and, uploaded these files into S3 bucket alongside the jsonpath file which will be used to create table in Redshift cluster.
-Deployed Amazon Redshift cluster, created required tables and, created IAM role to have identity verification, when trying to access redshift cluster. Pulled the data from S3 bucket to Redshift cluster by using “copy” command. 
-Deployed Quicksight and, connected to Redshift Cluster. Once the data in Quicksight, generated following visualizations to analyze the data.
-Price comparison chart for the following stocks: AMZN, GOOG.
-Price comparison chart for the rest of the stocks: MSFT, FB, APPL, VZ, ORCL, TWTR, NFLX, CSCO.
-Sample Portfolio Performance Chart:
 Assumed in January 2019, an investor bought $100,000 in the following stocks:
 25% MSFT,  5%AMZN,   5%GOOG,   25%APPL,   15%CSCO,   25% FB
 Provided a chart that shows how the portfolio value moved from the day the investor bough it until now. How much is this portfolio worth now?
