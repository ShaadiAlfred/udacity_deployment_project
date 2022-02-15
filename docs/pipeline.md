# Pipeline Process
1. CircleCI triggers and event when a new commit is pushed to the master branch in GitHub repo
1. CircleCI starts a linux instance, to build, run tests, and deploy
1. CircleCI installs necessary software:
    - `node: circleci/node@5.0.0`
    - `aws-cli: circleci/aws-cli@1.3.1`
    - `aws-s3: circleci/aws-s3@3.0`
    - `eb: circleci/aws-elastic-beanstalk@2.0.1`
1.  CircleCI setups the environment variables so `aws-cli` can deploy the code:
    - `aws-cli/setup`
    - `eb/setup`
1. Installing frontend dependencies
1. Building frontend
1. Installing backend dependencies
1. Building backend
1. Deploying backend (zipping contents of `udagram-api/www` directory, and uploading it with `eb`)
1. Deploying frontend (synching contents `udagram-fronted/www` to the s3 bucket with `aws s3`)
