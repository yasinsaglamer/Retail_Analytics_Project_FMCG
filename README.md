# 🚀 FMCG Retail Intelligence: AI-Ready Data Product on Microsoft Fabric

## 📌 Executive Summary
This project demonstrates a full-scale Data Engineering and BI implementation within the **Microsoft Fabric** ecosystem. Starting from a raw FMCG dataset (generated via Gemini for realistic simulation), I engineered a high-performance **Star Schema** designed specifically for **Generative AI (LLM) consumption**.

**The Mission:** To enable non-technical sales teams to interact with complex retail data using **Natural Language (AI Chatbots)**, reducing the time-to-insight from hours to seconds.

---

## 🏗️ Technical Architecture (The Medallion Journey)
The project follows the Medallion Architecture to ensure data quality and AI readiness:

1. **Bronze (Raw):** Direct ingestion of retail datasets into the Fabric Lakehouse in Delta format.
2. **Silver (Refined):** Data transformation using **PySpark**. This stage includes cleaning, schema enforcement, and handling nulls.
3. **Gold (Curated - Star Schema):** Creation of an optimized semantic model. Tables are organized into **Fact_Sales** and **Dimensions (Product, Store, Calendar, Geography)** to maximize AI query accuracy.



---

## 🤖 AI-Ready Semantic Modeling
A unique feature of this project is the **optimization for Natural Language Processing (NLP)**. To ensure a Chatbot can accurately provide insights:
* **Star Schema Implementation:** Minimized table joins to prevent AI "hallucinations" during querying.
* **Semantic Descriptions:** Every column in the Gold layer is enriched with metadata, helping AI agents understand business context (e.g., defining "OOS" as Out-of-Stock).
* **Pre-calculated Measures:** Complex DAX formulas are stored within the model so the AI doesn't have to calculate them on the fly.

---

## 🛠️ Tech Stack
* **Platform:** Microsoft Fabric (OneLake, Lakehouse, Data Factory)
* **Engineering:** PySpark, Spark SQL
* **Modeling:** Power BI Semantic Models (Star Schema)
* **AI:** Microsoft Fabric Copilot & LLM Integration

---

## 📊 Business Impact
* **Conversational Analytics:** Sales managers can ask, *"Which category had the highest stock-out rate in Istanbul last weekend?"* and get an instant answer.
* **Proactive Inventory:** Automated detection of inventory gaps across 5,000+ SKU/Store combinations.

---

## 👤 Author
**Yasin Saglamer**
* Statistics Student @ Yildiz Technical University (YTÜ)
* Business Intelligence Developer Intern @ Boost Intelligent Analytics
├── data_generation/    # Python scripts for synthetic dataset creation
├── notebooks/          # Fabric/PySpark notebooks for ETL processing
├── sql_scripts/        # Gold layer views and DDL scripts
├── power_bi/           # PBIX files and dashboard screenshots
└── README.md           # Project documentation
