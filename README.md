# dbt-databuildtool---netflix analysis

🍿 Netflix Data Pipeline Project with dbt, Snowflake, and BI Tools
This project demonstrates a modern ELT data pipeline using Netflix dataset with a fully functional stack:
Amazon S3 → Snowflake → dbt → BI tools (Power BI, Tableau, Looker Studio)

Inspired by the amazing work of Darshil Parmar. His content was instrumental in building this project and understanding dbt workflows in the real world. 🙌

🧠 Project Objective
To design and implement a production-grade data transformation pipeline using dbt on top of Snowflake, simulating a typical analytics engineering workflow with Netflix data. The output is served to BI tools for analysis and visualization.

📌 Architecture Overview
image

Layered Breakdown:
Raw Layer: Data from CSV loaded into Snowflake via Amazon S3
Staging Layer: Transformed and modeled using dbt (with version control, testing, and documentation)
Serving Layer: Final cleaned and analysis-ready tables available for visualization
🔧 Tools & Technologies
Layer	Tool/Service	Purpose
Extraction	CSV, Amazon S3	Ingest data into cloud
Storage	Snowflake ❄️	Data warehouse
Transformation	dbt (Data Build Tool)	SQL-based transformation, testing, and orchestration
Visualization	Power BI, Looker Studio, Tableau	BI and storytelling 📊
💡 Why ELT over ETL?
ETL: Transform before loading → High upfront processing & less flexibility
ELT: Load first, Transform in-warehouse → Leverages power of cloud data warehouses
With dbt, ELT becomes modular, scalable, and production-ready ⚙️
✅ Features
Cloud-based ELT architecture
dbt transformations with staging, intermediate, and serving models
Testing, documentation, and version control using dbt
BI integration for reporting
Clean, modular, and reusable SQL models
🏁 How to Run Locally
Clone the Repo
git clone https://github.com/yourusername/netflix-dbt-project.git
cd netflix-dbt-project
