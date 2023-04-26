# Snowflake Data Loading from Chess Streaming Data

## Purpose:

Building an end-to-end Data pipeline to collect useful information about streamers on chess.com, storing this data in S3 and modelling it on Snowflake



## How to Run This Project

Steps I followed to achieve the requirement:
1.	I have used Lichess API to extract chess data. In that Bersrek is a Python client for the Lichess API.
2.	Authentication is done with personal tokens and establishing a session.
3.	Post that I have obtained Blitz, Bullet, Rapid and Livestreaming leader boards. 
4.	Boto3 makes it easy to integrate your Python application, library, or script with AWS services including Amazon S3. 
5.	Connected to AWS using AWS access key and secret key.
6.	After that written script to automatically load the data pulled from API to S3.
7.	Configured storage integration object in snowflake to access S3 bucket
8.	Configured role and edited access policy in IAM and Snowflake, S3 connection is established.
9.	SQS Queue configuration:Using SQS, we can send, store, and receive messages between two different services by creating an intermediate queue instead of sending the messages directly.
10.	Loaded S3 file to snowflake tables using copy into command.
11.	Installed Airflow and done snowflake to airflow configuration.
12.	Airflow is basically used to Orchestrate the script to operate on timely basis. In this project it is to be operated every hour.


# Contact

https://www.linkedin.com/in/narrasravani/
