# GlueProject
part1: Preparation
1. Create IAM Role

2. Add S3 bucke in Lake Formation

3. Create catalog database

4. Grant the permissio to database and table in Lake Formation
   - why I need to grant the permission to database -> (case 1)[]
      - when I run the crawler to careate the table in catalog database, it needs the permission to catalog database
   - why I need to grant the permission to the tables -> (case 2)[]
      - when I want to delete the table, then I find I need the permission to deal with the table

part2: Create a Crawler
5. create table using crawler
- read the schema in s3 bucket 
- read the schema in RDB database (postgresql core)
  - create a connection to the RDB database

part3: Create a Glue Visual ETL Job
6. Build the ETL Job 
- Read the data from s3 bucket as format csv, save to s3 bucket as format json
- Read data from S3 json file, save to the RDS Postgres Database


part4: Create a Glue script ETL Job
- Read the data from s3 bucket as format csv, save to s3 bucket as format json

part5: How to solve the connection fail in Glue Job
- Read data from S3 json file, save to the RDS Postgres Database

7. Build the workflow on demand 

8. Build workflow the first trigger depend on the event that s3 update new folders
- Create cloudTrail for s3 event
- Create eventBridge Rule for AWS API Call CloudTrail

9. Incremental Glue Crawling using Amazon S3 event notification (SQS)

10. Test check the behavior of Crawler

11. Create workflow with hourly scheduled




# Glue Project in Terrafor
1. create catalog database

2. Grant Lake Formation permission

3. Create connection

4. Create Crawler to RDB database

5. Create Glue ETL job

6. Create Workflow
