# Infrastructure

## RDS (Postgres DB)
Postgres database.

## EC2
Elastic Beanstalk environment that manages an EC2 instance to run the backend which communicates with the database and the frontend. It runs the `udagram-api` app which is a NodeJS app.

## S3
S3 bucket that the public can read, to get access to the frontend app, `udagram-frontend`.
