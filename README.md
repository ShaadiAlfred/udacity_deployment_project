[![CircleCI](https://circleci.com/gh/ShaadiAlfred/udacity_deployment_project/tree/master.svg?style=svg)](https://circleci.com/gh/ShaadiAlfred/udacity_deployment_project/tree/master)

# Infrastructure
- RDS (Postgres DB)
- EC2
- S3

# App Dependencies
- NodeJS
- Ionic Frameword
- TypeScript
- sequelize
- express

# Pipeline Process
1. Installing frontend dependencies
2. Building frontend
3. Installing backend dependencies
4. Building backend
5. Deploying backend (zipping contents of `udagram-api/www` directory, and uploading it with `eb`)
6. Deploying frontend (synching contents `udagram-fronted/www` to the s3 bucket with `aws s3`)


# Config images
![Web capture_1-2-2022_223128_s3 console aws amazon com](https://user-images.githubusercontent.com/3685582/152055145-fec41a2b-e3ea-48c7-a6dd-694eb50cb252.jpeg)
![Web capture_1-2-2022_2274_console aws amazon com](https://user-images.githubusercontent.com/3685582/152055152-49a7ef87-c4ca-4ca2-9329-f80c56947c38.jpeg)
![Web capture_1-2-2022_22633_console aws amazon com](https://user-images.githubusercontent.com/3685582/152055164-fa894094-7d1f-4711-80f1-ce5c3ceee3e1.jpeg)
![Web capture_1-2-2022_2264_console aws amazon com](https://user-images.githubusercontent.com/3685582/152055166-63955ec8-338c-4794-afce-519246b52c72.jpeg)
![Web capture_1-2-2022_22537_console aws amazon com](https://user-images.githubusercontent.com/3685582/152055168-efdf6cef-268c-4500-bee0-f7527e49aadf.jpeg)
![Web capture_1-2-2022_2258_console aws amazon com](https://user-images.githubusercontent.com/3685582/152055173-7941be5d-32c2-4d49-8dc5-ea6383113691.jpeg)
![Web capture_1-2-2022_22433_console aws amazon com](https://user-images.githubusercontent.com/3685582/152055176-8342cddb-fa6f-4e76-a627-3f8030174821.jpeg)
![Web capture_1-2-2022_22417_console aws amazon com](https://user-images.githubusercontent.com/3685582/152055183-e98116c5-6a84-4673-bf60-ec3579a3a20d.jpeg)
![image](https://user-images.githubusercontent.com/3685582/152055886-560c0338-e297-4b20-9389-38a76cbbbe25.png)
