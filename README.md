# Smart City End to End Realtime Data Engineering Project

# Background
This project involves equipping a vehicle traveling from Central London to Birmingham with an IoT device to collect real-time data on GPS location, weather conditions, and accidents. The aim is to enhance route optimization, safety, and operational efficiency by providing live updates and insights to the driver and fleet management. This initiative represents a step towards smarter, more connected vehicle operations.

![image](https://github.com/user-attachments/assets/663f8166-1e00-46a7-a1fc-80d21ed9b541)

# Techstack
- AWS Athena
- AWS RedShift
- AWS Glue
- AWS S3
- Zookeeper
- Kafka
- Spark
- Docker
- Power BI
- Python3.8

# Architecture
![diagram drawio](https://github.com/user-attachments/assets/5c24eee8-82d5-4989-b519-5d8864c90815)
- Data Sources: Information from vehicles, GPS, cameras, weather, and emergency systems is collected.
- Apache Kafka: Data from various sources is ingested into Kafka for real-time processing, managed by Zookeeper.
- Apache Spark: Kafka streams the data to an Apache Spark cluster for processing. The Spark cluster is made up of one master and multiple worker nodes.
- AWS Integration:
    - AWS S3: Processed data is stored in Amazon S3.
    - AWS Glue: Glue crawlers scan and catalog the data stored in S3.
    - AWS Athena: Enables querying of data stored in S3.
    - Amazon Redshift: Serves as a data warehouse for structured data.
-  Data Analysis and Visualization: Data can be visualized using Tableau and Looker for business intelligence and reporting.
