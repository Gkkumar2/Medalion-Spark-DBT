# 🚀 Data Engineering Project: Spark, DBT, and Azure Cloud  

![Azure](https://img.shields.io/badge/Azure-Data%20Pipeline-blue?style=for-the-badge&logo=microsoft-azure)  
![Spark](https://img.shields.io/badge/Apache%20Spark-Big%20Data-orange?style=for-the-badge&logo=apache-spark)  
![DBT](https://img.shields.io/badge/DBT-Transformations-red?style=for-the-badge&logo=dbt)  

## 🌟 **Project Overview**  
This project implements a **Data Engineering pipeline** using the **Medallion Architecture** on **Azure Cloud**. It leverages **Apache Spark, DBT, and Azure Data Services** for **data ingestion, transformation, and analytics**.  

### **📌 Key Features**  
✅ **Medallion Architecture** (Bronze, Silver, and Gold layers)  
✅ **Automated Data Pipelines** using Azure Data Factory  
✅ **Spark-based Processing** with Databricks  
✅ **Transformation & Modeling** using DBT  
✅ **Secure Credentials Management** via Azure Key Vault  
✅ **BI & ML Ready Data** in the Gold Layer  

---

## 🏗 **Architecture Overview**  

### 🔷 **Medallion Architecture**  
- **🟤 Bronze Layer:** Raw data storage in Azure Data Lake  
- **⚪ Silver Layer:** Cleaned and transformed data  
- **🟡 Gold Layer:** Business-ready, aggregated data  

### 🔗 **Technology Stack**  
| Component | Service Used |
|-----------|-------------|
| **Cloud Provider** | Azure ☁️ |
| **Data Orchestration** | Azure Data Factory 🔄 |
| **Data Storage** | Azure Data Lake Gen2 📦 |
| **Processing Engine** | Azure Databricks (Spark) 🔥 |
| **Transformation** | DBT ⚙️ |
| **Database** | Azure SQL Database 🗄️ |
| **Security** | Azure Key Vault 🔑 |
| **BI & Analytics** | Power BI / Tableau 📊 |

---

## 🔄 **Data Flow Diagram**  

![Diagram](https://github.com/Gkkumar2/Medallion-Spark-DBT/blob/main/Docs/Database%20Schema%20Overview%20-%20Page%201%20(3).jpeg)

---

## 🛠 **Setup Instructions**  

### **1️⃣ Create Azure Resources**  
- **Azure Data Factory**: Used for **orchestration**  
- **Azure Databricks**: Spark-based processing  
- **Azure SQL Database**: Source database  
- **Azure Data Lake Gen2**: Storage for data layers  
- **Azure Key Vault**: Secure credentials storage  

### **2️⃣ Configure Azure Data Factory (ADF)**  
- Create **Linked Services** for:  
  - Azure SQL Database  
  - Azure Data Lake Storage (ADLS)  
  - Azure Databricks  
- Define **Pipelines** to copy data from SQL to **Bronze Layer**  

### **3️⃣ Set Up Databricks for Data Processing**  
- **Mount ADLS Storage** in Databricks using Azure Key Vault  
- Load **Bronze Layer** data and apply transformations  
- Write **transformed data** to **Silver and Gold Layers**  

### **4️⃣ Implement DBT for Data Transformation**  
- Configure **DBT models** for further transformations  
- Use `dbt run` to create **business-ready tables**  

### **5️⃣ Schedule Workflows**  
- Use **ADF triggers** to automate pipeline execution  
- Schedule **Databricks notebooks** for periodic transformations  

---

## 🎯 **Key Benefits**  
✔️ **Scalable** architecture for handling large datasets  
✔️ **Automated** ETL pipelines for seamless data flow  
✔️ **Secure & Optimized** with best cloud practices  
✔️ **Ready for BI & ML** applications  


🚀 **Happy Data Engineering!**  
