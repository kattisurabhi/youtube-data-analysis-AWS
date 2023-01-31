# Data Engineering on youtybe analysis on AWS

Performing analysis on the youtube videos which are structured and semi-structured based on categories and trending metrics. 

Dataset : https://www.kaggle.com/datasets/datasnaek/youtube-new

The dataset consists of several months of data on daily trending youtube videos. 
The data is up to 200 trending videos per day, and is included for 10 different regions. (IN, US, CA, GB, DE, FR, RU, MX, KR, JP)

Data of every region is stored in a separate file. 
Details of the video, title, description, number of likes, comment counts, etc, are in the CSV file. The catergory_id differs by area and is included in the JSON file of every region.


Project details and services used:

AWS IAM : Access management to use the services securely
Amazon S3 : Store the raw and transformed data 
AWS GLUE : Create database and crawlers on the data to form tables. 
           Create jobs that run automatically when an event occurs.
           Preprocess : CSV - Parquet through GLUE job. 
AWS Lambda : Serverless computing service. 
             create function to convert the data from json to parquet format. 
AWS Athena : understanding the data through querying. 
QuickSight : Visualise the data 
             




