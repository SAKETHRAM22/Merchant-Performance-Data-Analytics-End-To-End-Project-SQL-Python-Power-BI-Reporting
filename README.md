📦 Inventory & Vendor Performance Analysis
An end-to-end analytics pipeline built for a growing manufacturing business managing diverse product lines. This personal portfolio project demonstrates industry‑standard best practices in data ingestion, transformation, statistical analysis, and interactive dashboarding using anonymized transactional data.

📌 This is a personal portfolio project intended for demonstration purposes only.

📖 Overview
Domain: Manufacturing company handling general products
Data Scope: Multi‑million‑row CSV files for inventory, purchases, sales, and vendor invoices
Objective:
Identify stock inefficiencies
Reduce carrying costs
Enhance vendor management
🚀 Key Features
📥 Data Ingestion & Audit Logging

Ingestion/ingestion_db.py loads raw CSV files into a SQL database
Detailed logs captured in Logs/ingestion_db.log for full traceability
🔄 Data Transformation & Modeling

Combined SQL and Python workflows generate a clean, vendor‑level summary table
📊 Advanced Analytics & Statistical Testing

Jupyter notebooks perform EDA, feature engineering, and hypothesis testing on profit margins, stock turnover, and unsold inventory
📈 Interactive Dashboarding

Power BI report visualizes KPIs such as profit margins, stock‑to‑sales ratios, and reorder recommendations
Includes dynamic charts, tables, and KPI cards
🗂️ Modular, Scalable Structure

Clear separation of images, ingestion scripts, logs, and analysis notebooks
Easy onboarding for new collaborators or future extensions
📁 Project Structure
Dashboard/
│   images/
│   └── Dashboard_preview.png               # Power BI dashboard snapshot  
│   Vendor PerformanceDashboard.pbix        # Interactive Power BI file  

Ingestion/
│   ingestion_db.py                         # Script for loading raw data into DB  

Logs/
│   ingestion_db.log                        # ETL process logs  

Notebooks/
│   Vendor Performance Analysis.ipynb                      # Main EDA & insights  
│   Vendor Performance Analysis (Transformed).ipynb        # Data transformation & summary table  

.gitignore                                   # Files/folders ignored by Git  
README.md                                    # Project documentation (this file)  
requirements.txt                             # Python dependencies  
🛠️ Tech Stack & Dependencies
Python 3.x — pandas, numpy, SQLAlchemy, matplotlib, seaborn, scipy, statsmodels
SQL — PostgreSQL or SQLite
Jupyter Notebook — Interactive data exploration
Power BI — Dashboard creation & reporting
Logging — Built‑in Python logging module
Refer to requirements.txt for exact package versions.

⚙️ Setup & Installation
Clone the repository

git clone https://github.com/Saif907/vendor-performance-dashboard.git
cd vendor-performance-dashboard
Create & activate a virtual environment

python -m venv venv
source venv/bin/activate      # macOS/Linux  
venv\Scripts\activate         # Windows  
Install dependencies

pip install -r requirements.txt
Load raw data into the database

python Ingestion/ingestion_db.py
Explore analysis notebooks

jupyter lab
Vendor Performance Analysis.ipynb → EDA & insights
Vendor Performance Analysis (Transformed).ipynb → Data transformation & summary table
View the Power BI dashboard Open Power BI Desktop and load Dashboard/Vendor PerformanceDashboard.pbix

📊 Dashboard Preview
