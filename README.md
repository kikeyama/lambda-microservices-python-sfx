# Python Demo Lambda

A simple backend (read/write to DynamoDB) with a RESTful API endpoint using Amazon API Gateway.

# Setup

## Environment variables

`SIGNALFX_ACCESS_TOKEN`  
`SIGNALFX_TRACING_URL` as `https://ingest.us0.signalfx.com/v2/trace`

## Other AWS Services

### DynamoDB table

Create table and put some data.

### API Gateway

1. Create API Gateway as REST API
2. Select this function as backend service with **Lambda Proxy Integration**
3. Deploy the API

## Layer

`arn:aws:lambda:<REGION>:254067382080:layer:signalfx-lambda-python-wrapper:2`  

See: https://github.com/signalfx/lambda-layer-versions/blob/master/python/PYTHON.md  

For deitaled instruction, refer to: https://github.com/signalfx/lambda-python
