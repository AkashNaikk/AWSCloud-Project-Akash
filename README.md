# AWSCloud-Project-Akash
This project automates the collection, processing, and presentation of the City of Vancouver: Council of Voting Records using AWS cloud services. It includes a data pipeline, processing, and API to view voting data through a cloud-based solution.

**Project Overview:**
This project leverages AWS to collect, store, process, and visualize the City of Vancouver: Council of Voting Records. It automates the data processing using serverless technologies for scalability and cost-effectiveness.

**Objective:**
The primary objective of this project is to clean and structure the council voting records dataset for the City of Vancouver. By performing data wrangling, we aim to:

Provide a clean and usable dataset that can be used for analysis.
Facilitate the identification of voting trends, patterns, and possible alignments or divisions within the council.
Ensure accuracy for future policy-making analysis, public transparency, and civic engagement.

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

**Dataset:**
The dataset includes the following components:

Councilor Voting Records: Each council member's vote on resolutions, motions, and policies (Yes, No, Unattended).
Meeting Information: Date and agenda of each meeting.
Issue Categories: Broad topics discussed (housing, transportation, environment, etc.).
Vote Breakdown: Summary of the outcome for each vote (Passed/Rejected).
Attendance Records: Which councilors attended each session.
Resolutions Text: Full text of the resolutions and motions presented for voting.

**Methodology:**
**Data Collection:**
Extract data from official City of Vancouver council archives and meeting records.
Scrape or download structured voting data available on public portals.
Collect meeting agendas and minutes to ensure all relevant votes are captured.

**Data Assessment:**
Conduct an initial review to assess the quality and completeness of the data.
Identify issues such as missing votes, inconsistent formatting, and duplications across records.

**Data Cleaning:**
Remove incomplete, duplicate, or inconsistent voting records.
Standardize councilor names and voting statuses (e.g., Yes, No) to ensure consistency.
Resolve missing data through cross-referencing multiple sources.

**Data Transformation:**
Convert date formats to ensure consistency across the dataset.
Categorize the issues or agenda topics by grouping related motions.
Add derived features, such as councilor attendance rate and voting alignment with the majority.

**Data Consolidation:**
Merge records of council meetings, votes, and issues into a unified database.
Ensure each vote is properly linked to the relevant councilor and issue category for analysis.

**Documentation and Validation:**
Document the data wrangling steps, including any challenges faced and the approach to resolving them.
Validate the dataset by cross-checking with official city records and performing exploratory data analysis (EDA).

**Technologies Used**
- AWS Lambda
- Amazon S3
- Amazon RDS
- AWS Glue
- Amazon API Gateway
- Python

Dataset Identifier: Council of Voting Records
Data owner and Publisher: City of Vancouver
![image](https://github.com/user-attachments/assets/45f6559e-4299-4703-82ca-ca8342abe024)

The objects and folders within the bucket are created
![image](https://github.com/user-attachments/assets/e0241581-2217-4727-a598-6058db8b95cc)

![image](https://github.com/user-attachments/assets/86a30c75-3640-4695-8aa4-a3a04d612631)

**Review Data Quality**
Duplicates: Eliminate duplicate records.
Missing Values: Identify and handle any missing values in key columns.
Filter rows: Remove rows that are not relevant to the analysis, such as permits that are
not related to the construction.
Data Errors: Correct any errors in the data, such as incorrect dates or outliers.
![image](https://github.com/user-attachments/assets/bfbcbfe0-90e0-450c-8771-e3c7d12b1443)

**ETL Pipeline**
Data Source: S3 bucket
Transformations: Change Schema, Aggregation, Dynamic Transform

<img width="1191" alt="VotingETL" src="https://github.com/user-attachments/assets/3262dbb1-5db4-4304-aade-820baf43749a">

**Part 2 -**

This second part focuses on data protection, governance, and monitoring in the second phase of the City of Vancouver's Data Analytics Platform (DAP). It looks at technological ways to use AWS to provide strong security and adherence to data management laws. Applying the five pillars of the AWS Architecture framework, the study assesses the platform's execution and pinpoints areas in need of development. The security, optimization, and long-term sustainability of the DAP are guaranteed by the integration of data protection, governance, and monitoring with the AWS architecture.

Encryption keys are generated, managed, and stored securely by the AWS KMS service to protect data. Simpler yet potentially less secure are symmetric keys. Two different keys are needed for encryption and decoding with asymmetric keys. Lab jobs have access to sensitive procedures, including key administration. Multiple file versions are allowed by S3 versioning, while data flow is automated by replication rules.

![image](https://github.com/user-attachments/assets/dd8f8652-c78c-4589-9003-81784f28f66d)

![image](https://github.com/user-attachments/assets/3b7a27fe-3eb7-489e-bf7e-a5763628744e)

![image](https://github.com/user-attachments/assets/2220111b-1631-457a-9a7d-8274e02cab4b)

![image](https://github.com/user-attachments/assets/0a4ff6fa-4f35-4bc9-9575-15babc1da3fa)

**ETL Process: Glue**
1. Data Source – CSV.file from RAW
2. Transform – Detect Sensitive Data
3. Transform – Evaluate Data Quality
4. Conditional Router
5. Transform – Default Group
6. Transform – Change Schema
7. Save – Store Finalized Data

![image](https://github.com/user-attachments/assets/f08bbf7d-79c1-4e3f-af99-7959fd15ce06)

AWS CloudWatch for managing and monitoring a range of AWS services, with a particular emphasis on comprehending and monitoring metrics pertaining to service performance. They particularly keep an eye on cost-related variables in the billing area.

![image](https://github.com/user-attachments/assets/496a87fa-6258-42a0-badd-f65bfb09a168)

![image](https://github.com/user-attachments/assets/5cd9d385-f7e6-48bc-8ad6-265c61c627c3)

![image](https://github.com/user-attachments/assets/a30ae6a8-d00d-47dc-bec1-dcd4e957f3e8)

![image](https://github.com/user-attachments/assets/7080ef8c-7f35-473c-bbf1-41ab14120014)

The City of Vancouver's Data Analytic Platform (DAP) was created and put into use with the goal of improving public service management's data accessibility, transparency, and efficiency. The platform is built for efficiency and scalability, guaranteeing flexibility in response to changing needs. It incorporates essential AWS services including S3, Glue, Athena, and EC2. The project's cost estimate validates the viability of long-term deployment by showing a sustainable and economical method. 
