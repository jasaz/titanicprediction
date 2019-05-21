It's not easy to build external libraries eg. scikit learn with AWS Lambda. It requires a lot of work in terms of installing the necessary 
libaries in a directory in Amazon Linux container, mapping container volume to the host, zipping the lambda function with the libraries and uploading it.
Instead I am attempting to use AWS Fargate (serverless container) instead of AWS Lambda. the idea is to have APIGateway invoke Fargate which 
inturn build and infers the model in S3.

THis is a work in progress.
