# Belgian Traffic Accidents Data Pipeline

This project implements a comprehensive **ETL pipeline** for processing and analyzing a dataset of **Belgian traffic accidents**. The raw data is initially provided as a `.txt` file, which is uploaded to **AWS S3**. Using **AWS Glue ETL**, the data is cleaned and transformed into a compressed **Parquet** format, making it efficient and ready for analysis.

## Pipeline Overview
1. **Data Source**: The Belgian Traffic Accidents dataset (`.txt` file) is used.
2. **Amazon S3** object storage to store the **raw data**
3. **Catalog with AWS Glue Crawler**: **AWS Glue Crawler** is used to scan the **S3 data** and infer its **schema**, registering it in the **AWS Glue Data Catalog**.
4. **ETL Processing**: **AWS Glue ETL** cleans, transforms, and converts the raw data into a **Parquet** file format with **Snappy compression**, optimizing it for performance and storage.
5. **Amazon S3** is used again to store the clean **Parquet** file. Ready for analysis.


### Result
The transformed Parquet data is now accessible for analysis with tools like Amazon Athena, Power BI, and Python, enabling efficient and scalable insights.

