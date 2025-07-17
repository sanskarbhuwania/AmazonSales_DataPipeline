# **Real-Time Data Streaming with Kafka, AWS S3, Glue & Athena**

## 📌 **Project Overview**
This project showcases a real-time data pipeline that streams Amazon sales data using **Apache Kafka**, stores it in **AWS S3**, processes it with **AWS Glue**, and enables **SQL-based querying in Athena**. The goal is to build a scalable and efficient cloud-based data processing solution.

## ⚙️ **Tech Stack**
- **Apache Kafka** – Real-time message streaming
- **AWS S3** – Cloud storage for Kafka consumer output
- **AWS Glue** – Schema detection and ETL processing
- **AWS Athena** – SQL querying on structured data
- **Python** – Data ingestion and processing scripts
- **IAM Roles & Policies** – AWS access management

---

## 🚀 **Project Workflow**
1. **Kafka Producer** streams real-time Amazon sales data from a dataset.
2. **Kafka Consumer** ingests and writes data to an S3 bucket.
3. **AWS Glue Crawler** detects schema and structures data for querying.
4. **AWS Athena** enables SQL-based queries for data analysis.

---

## 🏗 **Setup & Execution**
### **1️⃣ Prerequisites**
- AWS Account with permissions for **S3, Glue, Athena**.
- Kafka installed on an **EC2 instance**.
- Python environment with required dependencies.

### **2️⃣ Steps to Run**
1. **Start Zookeeper & Kafka Server**  
   - Ensure Kafka is up and running on the EC2 instance.

2. **Create a Kafka Topic**  
   - Define a topic to publish and consume sales data.

3. **Run Kafka Producer**  
   - Streams Amazon sales data into Kafka.

4. **Run Kafka Consumer**  
   - Writes incoming data from Kafka to AWS S3.

5. **Configure AWS Glue & Athena**  
   - Create a Glue Crawler to recognize schema.
   - Use Athena to run SQL queries on the structured data.

---

## 🔥 **Key Challenges & Fixes**
### ⚠ **Kafka Server Crashes Due to High Resource Usage**
✔ **Fix**: Introduced a delay in the consumer to prevent overwhelming the broker.

### ⚠ **Glue Crawler Didn’t Create a Table in Athena**
✔ **Fix**: Updated IAM roles and permissions to allow Glue access to S3 and the Glue Catalog.

---

## 📊 **Results**
✅ Seamless real-time streaming from **Kafka → S3 → Glue → Athena**  
✅ Efficient **cloud-based storage** with optimized file writing strategy  
✅ **SQL-based querying** on live data for faster insights  

---

## 🎯 **Future Enhancements**
- **Apache Iceberg** for optimized data lake storage.
- **AWS Redshift Spectrum** for federated querying.
- **Kafka Streams** for real-time data transformations.

---

## 💡 **Contributions & Support**
Feel free to contribute, suggest improvements, or raise issues!  
📧 Contact: **kolusuvandana13@gmail.com**

---

