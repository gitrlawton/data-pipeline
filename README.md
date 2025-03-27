# Day 4: 30 Day DevOps Challenge

## Project: NBA Stats Pipeline with AWS DynamoDB and CloudWatch

This project is an exercise from the 30 Day DevOps Challenge. It demonstrates the creation of a data pipeline that collects NBA team statistics using the sportsdata.io API and stores them in AWS DynamoDB, with comprehensive logging using AWS CloudWatch.

## Project Overview

The project consists of two main Python scripts:

1. `nba_stats.py`: Core pipeline implementation for fetching and storing NBA statistics
2. `lambda_function.py`: AWS Lambda handler for serverless execution

## Features

### NBA Stats Pipeline (`nba_stats.py`)

- Fetches NBA team statistics from sportsdata.io API
- Stores data in DynamoDB with team-based partitioning
- Implements structured JSON logging
- Configures CloudWatch logging for monitoring
- Handles data type conversion for DynamoDB compatibility
- Provides automatic DynamoDB table setup

### Lambda Integration (`lambda_function.py`)

- Serverless execution of the data pipeline
- Error handling and status reporting
- HTTP response formatting for API Gateway integration

## AWS Services Used

- Amazon DynamoDB: For storing NBA team statistics
- AWS CloudWatch: For logging and monitoring
- AWS Lambda: For serverless execution
- AWS SDK (boto3): For AWS service interaction

## Monitoring

The pipeline includes comprehensive logging:

- JSON-formatted logs for structured data
- Console output for local development
- CloudWatch integration for production monitoring
- Error tracking and exception handling
