# Belgian Traffic Accidents Data Pipeline

This project implements a comprehensive **ETL pipeline** for processing and analyzing a dataset of **Belgian traffic accidents**. The raw data is initially provided as a `.txt` file, which is uploaded to **AWS S3**. Using **AWS Glue ETL**, the data is cleaned and transformed into a compressed **Parquet** format, making it efficient and ready for analysis.

## Pipeline Overview
1. **Data Source**: The Belgian Traffic Accidents dataset (`.txt` file) is uploaded to **Amazon S3**.
2. **ETL Processing**: **AWS Glue ETL** cleans, transforms, and converts the raw data into a **Parquet** file format with **Snappy compression**, optimizing it for performance and storage.
