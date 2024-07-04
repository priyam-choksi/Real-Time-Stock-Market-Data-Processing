### Real-Time Stock Market Data Processing with Kafka and AWS

---

## Project Overview
This project focuses on constructing a real-time data engineering pipeline for stock market data using Apache Kafka, Python, and various AWS services. The goal is to demonstrate an end-to-end implementation that collects, processes, stores, and queries stock market data in real-time, offering insights into the technical execution and scalability of data pipelines.

## Architectural Diagram
![Stock Market Kafka Real-Time Data Engineering Architecture](Architecture.jpg)

## Technologies Used
- **Python**: Primary programming language for scripting and automation.
- **Apache Kafka**: Used for building real-time data streaming pipelines.
- **Amazon Web Services (AWS)**:
  - **S3 (Simple Storage Service)**: Data storage solution.
  - **EC2 (Elastic Compute Cloud)**: Server hosting for Kafka and other processes.
  - **Glue**: ETL service for cataloging and processing data.
    - **Glue Crawler**: Automates the categorization of data into the Glue Catalog.
    - **Glue Catalog**: Metadata storage for data assets.
  - **Athena**: SQL querying service used for analyzing data directly in S3 using standard SQL.

## Dataset
This project is structured to work with any stock market dataset. The provided dataset includes processed stock indices, which is available on GitHub:

[Processed Stock Indices Dataset](https://github.com/priyam-choksi/Real-Time-Stock-Market-Data-Processing/blob/main/indexProcessed.csv)

## Implementation Details
1. **Data Collection**: Utilize Boto3 SDK to simulate real-time stock market data generation and ingestion into Kafka.
2. **Data Streaming**: Implement Kafka producers and consumers to handle the flow of data in real-time.
3. **Data Storage and Management**: Use AWS S3 for storing processed data, with Glue services to manage data cataloging and schema evolution.
4. **Data Querying**: Leverage AWS Athena for efficient querying capabilities on large-scale data stored in S3.

## Instructions for Setup and Execution
- Setup AWS services and configure Kafka on an EC2 instance.
- Ensure all services are interconnected and data flow is properly managed across different AWS components.
- Deploy the Python scripts to simulate data production and consumption processes.
- Regularly monitor system performance and adjust configurations as necessary to handle different data volumes and velocities.

---
