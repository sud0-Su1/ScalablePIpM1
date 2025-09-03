# Scalable Pipeline M1 – Olist Data Processing & Analytics

##  Overview  
This project implements a **scalable data pipeline** for processing, analyzing, and loading the popular Olist datasets into a data store or analytical engine. It demonstrates how to ingest raw CSV sources, perform transformations and enrichment, and make data analysis-ready—effectively supporting downstream analytics or BI tools.

---

##  Project Highlights  
- **Data Ingestion Notebook** (`DataIngestionToDB.ipynb`): Reads and processes raw Olist datasets (orders, payments, customers, etc.).  
- **ETL Logic**: Leverages Pandas and/or PySpark within the notebook to transform and clean datasets, enforcing schema consistency and handling missing values.  
- **SQL Integration**: Contains a `sql code` file for building analytical views, performing aggregations, and preparing dataset relationships.  
- **Architecture Diagram** (`Architecture Diagram.excalidraw`): Visual overview of data flow from CSV ingestion to final storage/analytics layer.  
- **Sample Data & Visuals**: Includes raw Olist CSVs and `image.png` for data samples or dashboard previews (optional).

---

##  Repository Structure

├── Architecture Diagram.excalidraw # Visual pipeline architecture
├── DataIngestionToDB.ipynb # Notebook for ETL and ingestion
├── sql code # SQL script(s) for downstream queries
├── image.png # Sample data snapshot or diagram
├── olist_*.csv # Olist raw datasets (orders, customers, reviews, etc.)
└── README.md # Project overview (this document)


---

##  Getting Started

1. **Setup Environment**  
   - Recommended: Python 3.8+ with Jupyter, Pandas (or PySpark), and database client (e.g., SQLite, PostgreSQL).  
   - Optional: Install with `pip install -r requirements.txt` if available.

2. **Data Ingestion**  
   - Open and run `DataIngestionToDB.ipynb`.  
   - The notebook showcases reading raw CSVs (`olist_*.csv`), performing data transformations, and loading data into a destination (e.g., local PostgreSQL or SQLite database).

3. **Run SQL Analytics**  
   - Use the provided `sql code` script to execute analytical queries—such as order trends, customer activity, average payments, or review summaries.

4. **Explore the Architecture**  
   - View the `Architecture Diagram.excalidraw` for a visual representation of the pipeline flow—from files through ingestion, transformation, and storage.

---

##  Intended Applications

This pipeline can serve as the backbone for:
- **Dashboarding** (e.g., Power BI, Tableau, or Plotly)  
- **Business Intelligence** (sales trends, customer engagement, payment performance)  
- **Scalable Refactoring** (porting to PySpark, Airflow, Azure Databricks)  
- **Machine Learning Pipelines** (predictive analytics based on customer and order history)

---

##  Future Enhancements
- Execute the pipeline over a production-grade engine (e.g., Spark, Databricks, or Prefect/Airflow orchestrator).  
- Implement incremental ingestion to support real-time or near-real-time data updates.  
- Extend with data validation, monitoring, and lineage tracking.  
- Add visualization dashboards or performance benchmarks.


**This project embodies the core of scalable data engineering—taking raw datasets through ingestion, transformation, and making them ready for analytics.**


