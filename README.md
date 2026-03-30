# 🛒 FMCG Retail Analytics: End-to-End AI-Ready Data Intelligence

## 📌 Project Overview
This project focuses on building a modern, end to end data lifecycle for the **Fast Moving Consumer Goods (FMCG)** sector. Using **Microsoft Fabric**, I have transformed raw, synthetic sales and inventory data into a highly optimized **Star Schema** semantic model.

### The "AI First" Approach
The primary goal of this project is to move beyond static dashboards. By structuring the data into a clean Star Schema, the model is designed to be **AI-Ready**. This allows sales teams to interact with their data using **Natural Language (Chatbots)** to gain instant insights such as identifying stock outs or regional sales peaks without needing to write a single line of SQL.

---

## 🛠️ Tech Stack & Tools
* **Data Orchestration:** Microsoft Fabric (Data Factory & Lakehouse).
* **Storage & Processing:** Delta Tables (Spark SQL & PySpark).
* **Modeling:** Star Schema (Medallion Architecture: Bronze → Silver → Gold).
* **Business Intelligence:** Power BI & Fabric Copilot for AI-driven insights.

---

## 🏗️ Architecture
1.  **Ingestion (Bronze):** Raw sales, inventory, and product data stored in Delta format.
2.  **Transformation (Silver):** Data cleaning, deduplication, and relationship mapping using PySpark.
3.  **Gold Layer (Semantic Model):** Optimized Star Schema consisting of:
    * **Fact Tables:** Sales, Inventory Snapshots.
    * **Dimension Tables:** Product (SKUs), Store, Calendar, and Geography.
4.  **AI Layer:** Integration with LLMs/Copilot to allow conversational analytics for sales stakeholders.

---

## 🚀 Current Progress (Work in Progress 🚧)
- [x] **Data Generation:** Synthetic FMCG dataset script completed.
- [x] **Fabric Setup:** Lakehouse environment and workspace configured.
- [ ] **ETL Pipelines:** Development of Silver and Gold layer transformations.
- [ ] **Semantic Modeling:** Implementing the AI optimized Star Schema.
- [ ] **AI Integration:** Testing natural language queries against the semantic layer.

---

## 📊 Key Business Insights Target
* **Sales Performance:** YoY/MoM growth and regional heatmaps.
* **Inventory Intelligence:** Real time tracking of Out of Stock (OOS) rates and replenishment alerts.
* **AI Conversational Analytics:** Enabling queries like: *"Which stores in Istanbul are at risk of running out of beverage SKUs by Friday?"*

---

## 📂 Repository Structure
```text
├── data_generation/    # Python scripts for synthetic dataset creation
├── notebooks/          # Fabric/PySpark notebooks for ETL processing
├── sql_scripts/        # Gold layer views and DDL scripts
├── power_bi/           # PBIX files and dashboard screenshots
└── README.md           # Project documentation
