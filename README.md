# Tokyo Olympics Data Analytics Pipeline on Azure

## 📊 Project Overview

This project demonstrates an end-to-end data engineering solution built on Microsoft Azure, analyzing the Tokyo 2021 Olympics dataset. The pipeline extracts data from GitHub, processes it through Azure cloud services, and delivers interactive visualizations through Power BI dashboards.

**Key Metrics:**
- 🏃 **11,000+** Athletes analyzed
- 🏅 **339** Olympic events covered
- 🌍 **206** Countries represented
- 📈 **50+** Data-driven insights generated

---

## 🏗️ Architecture

![End-to-End Data Pipeline](end-to-end data pipeline using azure.png)

The architecture follows a modern cloud data engineering approach with clear separation between raw and transformed data layers.

---

## 🛠️ Technologies Used

| Component | Technology | Purpose |
|-----------|-----------|---------|
| **Data Source** | GitHub | Host raw CSV files (Athletes, Coaches, Medals, Teams, Entries) |
| **Orchestration** | Azure Data Factory | Automate data extraction and pipeline workflows |
| **Storage** | Azure Data Lake Gen2 | Store raw and transformed data layers |
| **Processing** | Azure Databricks (PySpark) | Data transformation, cleansing, and enrichment |
| **Data Warehouse** | Azure Synapse Analytics | SQL-based analytics and data warehousing |
| **Visualization** | Power BI | Interactive dashboards and reporting |

---

## 📁 Dataset

The project uses the following Tokyo Olympics CSV files:

- **Athletes.csv** - Athlete information (name, country, discipline)
- **Coaches.csv** - Coaching staff details
- **EntriesGender.csv** - Gender distribution across sports
- **Medals.csv** - Medal counts by country and event
- **Teams.csv** - Team compositions and countries

---

## 🔄 Data Pipeline

### 1️⃣ **Data Extraction**
Azure Data Factory extracts raw CSV files from the GitHub repository and loads them into the **Raw Data Layer** in Azure Data Lake Gen2.

### 2️⃣ **Data Transformation**
Azure Databricks processes the raw data using PySpark:
- Data cleansing (handling nulls, duplicates)
- Schema standardization
- Data enrichment and aggregations
- Quality validation checks

Transformed data is stored in the **Transformed Data Layer** in ADLS Gen2.

### 3️⃣ **Data Warehousing**
Azure Synapse Analytics ingests the transformed data for:
- Efficient SQL-based querying
- Star/snowflake schema modeling
- Advanced analytics and aggregations

### 4️⃣ **Visualization**
Power BI connects to Synapse Analytics to create:
- Medal distribution dashboards
- Country performance analysis
- Gender participation trends
- Athlete and event statistics

---

## 📂 Repository Structure

```
tokyo-olympic-azure-project/
│
├── README.md                              # Project documentation
├── end-to-end data pipeline using azure.png  # Architecture diagram
│
├── data/                                  # Raw CSV files
│   ├── Athletes.csv
│   ├── Coaches.csv
│   ├── EntriesGender.csv
│   ├── Medals.csv
│   └── Teams.csv
│
├── notebooks/
    └── Tokyo Olympic Transformation.ipynb  # Databricks PySpark notebook

```

---

## 📊 Key Insights Delivered

- **Medal Distribution:** Top 10 countries by gold, silver, and bronze medals
- **Gender Representation:** Male vs. female athlete participation across sports
- **Discipline Analysis:** Most competitive events by number of participants
- **Country Performance:** Comprehensive country-level statistics
- **Trend Analysis:** Historical comparison capabilities (when extended)

---

## 🎯 Learning Outcomes

This project demonstrates proficiency in:
- ☁️ Cloud-native data engineering on Azure
- 🔄 Building scalable ETL/ELT pipelines
- 🐍 Big data processing with PySpark
- 🗄️ Data warehousing and SQL analytics
- 📊 Business intelligence and data visualization

---

## 🔐 Security & Best Practices

- **Service Principals** used for authentication between services
- **Azure Key Vault** for storing secrets and connection strings
- **RBAC** implemented for access control
- **Data encryption** at rest and in transit (ADLS Gen2)
- **Monitoring** via Azure Monitor and Log Analytics

---

## 📈 Future Enhancements

- [ ] Implement incremental data loading
- [ ] Add data quality monitoring with Great Expectations
- [ ] Automate end-to-end pipeline with Azure DevOps
- [ ] Implement real-time streaming analytics with Event Hubs
- [ ] Add machine learning models for performance prediction
- [ ] Create REST API using Azure Functions for data access

---

## 👨‍💻 Author

**Yazid ABDELMONEM SIED AHMED**

- 📧 Email: abdelmonem.yazid@gmail.com
- 💼 LinkedIn: [Yazid ABDELMONEM SIED AHMED](https://linkedin.com/in/yazidabdelmonem)
- 🐙 GitHub: [yzdpirate28](https://github.com/yzdpirate28)

---

## 📝 License

This project is open-source and available under the MIT License.

