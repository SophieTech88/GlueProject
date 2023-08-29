# GlueProject
1. Create IAM Role

2. Add S3 bucke in Lake Formation

3. Create catalog database

4.Grant the permissio to database and table in Lake Formation

5. create table using crawler
- s3 bucket
- RDB database

6. Build the ETL Job : Read data from S3 json file to the RDS Postgres Database

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
