# Modern Data Architectures on AWS

The use of a **data lake** as the central repository in a modern data architecture on AWS. Amazon S3 is the preferred storage service for building data lakes due to its scalability, durability, and cost-effectiveness.

Data lakes are integrated with purpose-built data stores and processing tools:

- Amazon Redshift, a fully managed data warehouse for SQL-based analytics.
- Amazon OpenSearch, a purpose-built data store for search and analytics. 
- Amazon EMR is a service for running big data processing frameworks like Spark and Hadoop.
- Amazon Aurora is a relational database engine built for the cloud.
- DynamoDB, a non-relational database designed for high-performance applications.
- Amazon SageMaker is an AI/ML service for building, training, and deploying machine learning models.
- AWS Lake Formation simplifies the process of setting up, securing, and managing data lakes. It helps catalog data, classify it, and enforce security policies for different types of access.

## Data Pipeline Stages

The ingestion layer brings data from various sources into the data lake. AWS provides purpose-built tools for ingesting different data types like AppFlow, Kinesis, and DMS.

The storage layer comprises two sub-layers. the **data storage layer** provides durability, scalability, and cost-effective storage. Amazon S3 and Redshift are used to create a unified storage layer.

The **catalog layer** stores business and technical metadata about the datasets, crucial for data governance and discovery. AWS Glue and Lake Formation work together to collect, store, and manage this metadata.

The processing layer prepares data for consumption by transforming, cleaning, and enriching it. Data in the data lake is typically processed using one of three main approaches:

- SQL based.
- Big data based.
- Real-time based.
 
 The consumption layer provides scalable and performant access to the processed data for various use cases. It allows different users across the organization to access data and supports various analysis methods:

- SQL queries.
- BI dashboards.
- Machine learning tools.
## Streaming Analytics Pipelines

Producers are integrations that collect data from a source and feed it into a stream, consumers process the records from the stream.

> AWS Kinesis and CloudWatch are two tools used for streaming pipelines.

## Amazon EMR

Amazon EMR is a managed cluster platform that simplifies the use of big data frameworks like Spark and Hadoop on AWS. EMR provides flexibility in choosing frameworks, applications, and storage options based on specific data processing needs.

- Quick cluster launch and deployment.
- Easy cluster resizing and scaling.
- Simplified management of big data frameworks.
