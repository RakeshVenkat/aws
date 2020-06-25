## Lambda:
A AWS lambda works using triggers.

A node service can be invoked via a trigger.

example: a lambda service can be a node.js code example that can be invoked by multiple triggers like uploads on S3.

Example:
Create an object in S3 -> triggers event -> Lambda
Upload an object in S3 -> triggers event -> Lambda
Copy an object in S3 -> triggers event -> Lambda

Note: There can be multiple Triggers using the same source like an S3.

There are multiple options of S3 that can trigger events in Lambda: POST, PUT, COPY object; Delete objects in S3; Restore from Glacier;

Source -> Lambda -> Destination

Source Trigger:

    API gateway
    CloudWatch Logs
    DynamoDB
    ......
    S3
    .....

Destination configuration:

Source:
    Async invocation
    Stream invocation

Condition:
    On failure
    On success

Lambda Destinations Type:
    SNS Topic
    SQS Topic
    Lambda Function
    Event Bridge Bus

Destination:
    DynamoDB

## S3:
Upload an object in S3.
Note: Upload object != Copy.
Copy an object from one S3 to another S3.

## Cloud Watch Logs:
Cloud watch logs are accessible with events refereshed every 3 seconds with logs.

## Cloud watch monitoring:
Cloud watch monitoring has all the logs necesary with refresh intervals of: 1h, 3h, 12h, 1d, 3d, 1w, custom.
