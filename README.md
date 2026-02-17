📊 Bank Marketing Campaign Analysis (PostgreSQL)  

📌 Project Overview  

This project analyzes 40,000+ customer records from a bank marketing campaign to answer a key business question:  

  Why do some customers subscribe to a term deposit while others don’t?  

The focus was not just querying data — but transforming raw, messy data into structured, analysis-ready tables using PostgreSQL.  

🛠 Tools & Technologies  
- PostgreSQL  
- SQL (CTEs, Window Functions, Aggregations)  
- EXPLAIN ANALYZE  
- Index Optimization   

🧱 Data Challenges Identified  
The raw dataset contained:  
- Numbers stored as TEXT  
- "unknown" values across key categorical columns  
- Misleading values (e.g., 999 in pdays)  
- No indexing for performance  
- No proper data type enforcement  

🔄 Data Preparation & Modeling  
✔ Created separate raw and cleaned tables  
✔ Converted TEXT fields into proper numeric data types  
✔ Replaced “unknown” values with NULL  
✔ Transformed yes/no fields into BOOLEAN  
✔ Added indexes for performance optimization  
✔ Built reusable reporting VIEW  

📊 Analysis Performed  
- Segment-wise conversion rate analysis  
- Campaign effectiveness evaluation  
- Contact frequency vs success rate  
- Economic indicators impact (Euribor rate)  
- Customer segmentation using CTEs & RANK()  

🚀 Performance Optimization  

Created indexes on high-filter columns

Compared execution plans using EXPLAIN ANALYZE

Observed Bitmap Heap Scan improvements

🔎 Key Business Insights

- Students showed one of the highest conversion rates  
- Longer call duration increased subscription probability  
- Fewer campaign contacts improved success rates  
- Economic indicators influenced customer behavior  

📸 Sample Outputs

Segment-wise conversion analysis

Query optimization plan (Bitmap Heap Scan via EXPLAIN ANALYZE)

📂 Repository Structure
/data-cleaning.sql
/analysis-queries.sql
/optimization.sql
/views.sql
/README.md

💡 What This Project Demonstrates

Strong SQL fundamentals

Data cleaning & normalization skills

Business-oriented analytical thinking

Query performance optimization

Structured database design approach

🔗 Author

Sarita Singh
Aspiring Data Analyst | SQL | PostgreSQL

Your Name
Aspiring Data Analyst
Open to collaboration and opportunities
