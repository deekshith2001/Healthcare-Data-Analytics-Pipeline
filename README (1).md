# Healthcare Data Pipeline

## **Overview**
The Healthcare Data Pipeline project is an advanced implementation designed to create a scalable and efficient data processing system for large healthcare datasets. Using tools like Apache Spark, Amazon S3, and Power BI, this pipeline transforms raw data into actionable insights, ensuring compliance with healthcare regulations and delivering high-performance analytics.

---

## **Tech Stack**
- **Data Lake**: Amazon S3
- **Data Source**: PostgreSQL
- **Data Read Storage**: MySQL on Amazon RDS
- **Processing Layer**: Apache Spark on Amazon EMR
- **Visualization**: Power BI

---

## **Architecture**
This pipeline follows a multi-layered architecture to ensure smooth data flow and analytics capabilities.

![Architecture](https://github.com/minhky2185/healthcare_data_pipeline/blob/main/images/architecture_2.png)

1. **Raw Zone**:
   - Data is ingested from PostgreSQL into the raw zone of the S3 data lake.
2. **Cleansed Zone**:
   - Raw data is cleaned and standardized to ensure data accuracy.
3. **Curated Zone**:
   - Cleansed data is transformed into a report-ready format and stored in the curated zone.
4. **Data Publishing**:
   - Data is published to MySQL on Amazon RDS for optimal report performance.
5. **Visualization**:
   - Power BI dashboards are created using the data in MySQL to generate insights and trends.

---

## **Data Source**
The dataset used in this project is sourced from the [CMS Provider Summary](https://data.cms.gov/provider-summary-by-type-of-service) and includes Medicare Part D data.

### **Database Tables**:
- **Prescriber_drug**: ~25M rows
- **Prescriber**: ~1.1M rows
- **Drug**: ~115K rows
- **State**: ~30K rows
- **Total Size**: ~10 GB

---

## **Visualization**
Interactive dashboards provide valuable insights into Medicare data.

### **Sample Dashboards**:
#### Drug Report
![Drug Report](https://github.com/minhky2185/healthcare_data_pipeline/blob/main/images/drug_report.png)

#### Prescriber Report
![Prescriber Report](https://github.com/minhky2185/healthcare_data_pipeline/blob/main/images/prescriber_report.png)

---

## **Key Features**

### **Scalability**:
- Handles datasets exceeding 10 GB efficiently.
- Modular design enables seamless integration of additional data sources.

### **Efficiency**:
- Optimized ETL workflows using Apache Spark and partitioning.
- Streamlined data transformations for quick insights.

### **Flexibility**:
- Easily adaptable for new reporting requirements or data sources.
- Real-time reporting capabilities via Power BI.

### **Cost Optimization**:
- Resource tuning on Amazon EMR minimizes operational costs.
- Effective use of S3 storage tiers for cost-efficient data storage.

---

## **Learning Achievements**

### **Apache Spark**:
- Mastered Spark's components and operations.
- Optimized Spark jobs using partitioning and resource tuning.
- Built end-to-end ETL pipelines with Spark.

### **AWS**:
- Deployed Spark on Amazon EMR for distributed data processing.
- Monitored EMR cluster utilization to enhance performance.

### **Project Setup**:
- Configured logging mechanisms for Spark applications.
- Tested and debugged workflows in local mode before cluster deployment.

---

## **Challenges and Solutions**

### **Challenge 1**: Processing large datasets efficiently.
**Solution**: Implemented Spark-based partitioning and distributed processing to reduce runtime and memory overhead.

### **Challenge 2**: Ensuring data quality and consistency.
**Solution**: Developed robust cleaning and validation mechanisms during ETL stages.

### **Challenge 3**: Managing cloud infrastructure costs.
**Solution**: Optimized EMR cluster configurations and utilized S3 tiered storage for cost savings.

---

## **Future Enhancements**
- **Real-Time Analytics**: Incorporate Kafka and Spark Streaming for real-time data processing.
- **Advanced Dashboards**: Add more visualization tools like Tableau or Looker.
- **Predictive Analytics**: Build models for trend forecasting and anomaly detection.
- **Security Enhancements**: Implement encryption and IAM roles for data security.

---

## **Getting Started**

### **Prerequisites**:
- AWS account with EMR, S3, and RDS enabled.
- PostgreSQL database with sample Medicare data.
- Power BI desktop application.

### **Setup Steps**:
1. Configure Amazon S3 buckets (`raw`, `cleansed`, and `curated` zones).
2. Load the provided dataset into PostgreSQL.
3. Deploy Spark on EMR and execute the ETL pipeline.
4. Publish the curated data to MySQL on RDS.
5. Connect Power BI to MySQL and build interactive dashboards.

---

## **License**
This project is licensed under the MIT License, allowing you to freely use, modify, and distribute the code with proper attribution. Refer to the `LICENSE` file for detailed terms.

---

## **Connect With Me**
- **Email**: [deekshithsaiteja25@gmail.com](mailto:deekshithsaiteja25@gmail.com)
- **LinkedIn**: [linkedin.com/in/deekshithdatasciencedataanalytics](https://www.linkedin.com/in/deekshithdatasciencedataanalytics)

---

Feel free to explore, contribute, or reach out for any collaboration opportunities!
