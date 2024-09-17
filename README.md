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

