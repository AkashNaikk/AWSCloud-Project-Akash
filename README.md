# AWSCloud-Project-Akash
This project automates the collection, processing, and presentation of the City of Vancouver: Council of Voting Records using AWS cloud services. It includes a data pipeline, processing, and API to view voting data through a cloud-based solution.

**Project Overview:**
This project leverages AWS to collect, store, process, and visualize the City of Vancouver: Council of Voting Records. It automates the data processing using serverless technologies for scalability and cost-effectiveness.

**Features:**
- **Automated Data Ingestion:** Collects voting records via AWS Lambda and stores them in an S3 bucket.
- **Data Processing**: Cleans and structures the data using AWS Glue.
- **API**: Provides an API endpoint (via AWS API Gateway and Lambda) to fetch and view voting data.
- **Storage**: Uses Amazon S3 for data storage and Amazon RDS for structured data queries.

**AWS Architecture**
The architecture includes the following AWS services:
- **Amazon S3**: For storing raw and processed voting data.
- **AWS Lambda**: For executing serverless functions that process and expose data.
- **Amazon RDS**: For storing structured voting data that can be queried.
- **AWS Glue**: For ETL (Extract, Transform, Load) data processing.
- **Amazon API Gateway**: For exposing the data through RESTful APIs.

**Technologies Used**
- AWS Lambda
- Amazon S3
- Amazon RDS
- AWS Glue
- Amazon API Gateway
- Python
