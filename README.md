Job-Market-Analysis/
├── Data from jobsdb website (Data, Bangkok, Date: 7/6/2025)/
│   └── Jobsdb_Raw.csv
└── Power Query (Power BI)
|	└──Clean Jobsdb_Raw.csv
|		└──Remove Column and Row (unusable data)
|		└──Rename Column
|		└──Merge Column
|		└──Split Column
|		└──Change annual salary information
|	└──Export Jobsdb_Raw.csv to Jobsdb_to_SQL.csv by DAX Studio
├── sql/
│   	└──Clean Jobsdb_to_SQL.csv
|		└──Clean Salary 
|			└──Create Table for look --- 'Clean_Salary Table'
|			└──Update Salary (USD to THB and Salary is stuck in the column with the text)
|			└──Remove Column
|		└──Position Grouping
|			└──Add Column for Group by Position ---'Positions_Group Column'
|			└──Create Table for look --- 'Group_Positions Table'
|			└──Update 'Position_Group Column' --- GroupPosition.text
|		└──Industry Grouping
|			└──Add Column ---'Industry Column'
|			└──Create Table for look --- 'GrouebyCompany_to_Industry Table'
|			└──Update 'Industry' Column --- GrouebyCompany_to_Industry.text
|		└──Update Salary by Position Group --- SalaryEstimate.text
|		└──See Tools Requirement --- Tools.xlsx
|	└──Export Jobsdb_to_SQL.csv to Jobsdb_final.csv
├── Dashboard (Power BI)/
│   └── DataJobs_from_Jobsdb.pbix
│   └── DataJobs_from_Jobsdb.pdf
├── LICENSE
├── .gitignore
├── README.md
## 🧠 Key Insights

- 💼 **Top 3 Positions in Demand**:  
  - Business Development
  - Business Analyst 
  - Sales Manager 

- 💸 **Average Salary Range (Data, Bangkok)**:  
  - 58000 THB / Month  

- 💼 **All open positions**:
  - 5070 positions

- 💸 **Top 3 industries with the most job openings**:  
  - Recuitment
  - travel Tech
  - Banking 

- 💼 **Top 3 Tools Requirement**:  
  - English
  - Excel
  - SQL


## ▶️ How to Use

1. Load `Jobsdb_Raw.csv` into Power BI
2. Clean the data using Power Query (see steps)
3. Export to `Jobsdb_to_SQL.csv` using DAX Studio
4. Run SQL scripts in `/sql/` to clean & transform
5. Load `Jobsdb_final.csv` into Power BI dashboard
