(https://simplonline.co/classrooms/6147353f-c0ac-4066-abba-b879be17ed4f/briefs/2260db57-d372-4d24-baa1-69cfd3b43f2f)

The company wants to publish anonymized sales data in an Open Data framework in order to strengthen its transparency and encourage collaborations. This database must be derived from the Data Warehouse while respecting the regulations on confidentiality and trade secrets. You are responsible for preparing the database that will be exposed in Open Data. The mission will result in a dual data structure: an accessible and standards-compliant Open Data base, and a data warehouse optimized for strategic analyses, providing the company with the means to better understand and exploit its data.

Teaching methods
Work requested:

1- Carry out technical and regulatory monitoring of the various constraints associated with Open Data, best practices for secure dissemination of data in Open Data. Identify the requirements concerning: * GDPR Principles * The various techniques for protecting personal data (anonymization, pseudonymization, etc.). * Data security to prevent leaks of sensitive information. * Statistical confidentiality to protect aggregated data.

2- Modeling and Implementation of the Data Warehouse: Centralize data, define fact and dimension tables, apply security rules.

3-Set up an extraction pipeline from the Data Warehouse to the Open Data base, applying transformations to guarantee anonymity.

4-Create the Open Data base, Implement the extraction and aggregation requests to feed the base.


Deliverables
1. Structured and optimized data warehouse: Constellation of fact tables and dimensions with specific data marts. 2. Open Data database: Database ready for public sharing, secure and compliant with data protection requirements. 3. Documentation: Technical monitoring document related to OpenData, Security and GDPR Compliance

Project context
You work as a junior data engineer in a large national group that wants to enhance its data by improving its accessibility and optimizing its structure for advanced analyses.

​

In this context, the company has set several key objectives for this year:

I. Optimization of internal data to provide business teams (sales, inventory, etc.) with more precise and faster analyses, allowing a better understanding of supplier trends and performance.

​

II. Provision of data in Open Data to meet transparency requirements and promote innovation.

To achieve these goals, you are responsible for organizing and transforming data to meet two needs:

​

I- a data warehouse optimized for business analysis:

​

1- Data Splitter + ETL script:

o Apply a Data Splitter script on the provided dataset to split the data facilitating the ETL process.

o Set up an ETL process, manage missing values ​​to maintain quality.

o Load data into the SQL warehouse, optimizing the ETL job for performance (subjobs, error handling, etc.).

2- Constellation schema modeling: Organize sales and inventory data into fact and dimension tables.

o Dimension tables: Create tables for dates, products, customers, suppliers, and carriers.

o Fact Tables: Set up SalesFact and InventoryFact tables for multidimensional analysis.

3- Creation of specific Data Marts: Build data marts to facilitate team analyses:

o Sales Data Mart (transactions, products, customers).

o Inventory Data Mart (products, suppliers, stock levels).

​

II- a publicly accessible Open Data base:

​

1- Modeling of the Open Data database:

​

o Design a data model suitable for public sharing by defining the target schema and the necessary relationships with the warehouse data.

2- Creation and feeding of the Open Data base:

o Implement extraction and aggregation queries to transform raw data into accessible and understandable data.

o Prepare the basis for sharing in Open Data in appropriate formats (CSV or other) and implement quality controls to ensure data consistency.

​

III- Security and GDPR Compliance (Bonus)

1- Indexing and optimization: Add indexes and partition tables to improve query performance, justifying each optimization performed.

2- Data protection policies:

o Identify and protect sensitive data (customer data) (with measures such as encryption, pseudonymization or others)

o To ensure compliance with the GDPR, propose measures to meet user rights (access, rectification, deletion).