# CASE STUDY
# Client Background: 
  Our client, a leader in staffing solutions, provides a variety of hiring services such as remote staffing, direct hire recruiting, contract staffing, retained search, and payrolling solutions.
  They cater to multiple industries, including accounting, legal services, support services, lending services, commercial banking, risk management, marketing, and sales. 
  The company not only recruit employees for its own needs but also places candidates with other organizations.
# Challenges: 
  The client faced significant difficulties in managing and tracking their staffing operations using Excel sheets.
  
  **Key challenges included:**
  1. Monitoring the status of employees across various stages of hiring and placement.
  2. Tracking hiring activities on a particular timeframe wise.
  3. Generating detailed reports related to finance, employee placement, and communication tracking (calls, emails, etc.).
Additionally, while the client used Bullhorn as a recruiting portal for manual data entry and reporting, the platform's built-in reports did not meet their growing and customized reporting needs.
# Solution: 
To resolve these challenges, we developed a comprehensive reporting solution using Power BI. The solution includes interactive charts, visuals, and tables that allow the client to monitor staffing metrics and performance based on user-defined timeframes.
Key Features of the Solution:

 **Data Integration:**
 1. Data was fetched from the Bullhorn portal using Python scripts and processed through an ETL pipeline.
 2. The transformed data was stored in a MySQL database, which serves as the backend for Power BI reporting.

**Interactive Power BI Reports:**
  The first report developed, the "Activity & Performance" report, tracks various aspects of staffing activity. It includes:
 1. Candidate Activity
 2. Sales Contact Activity
 3. Job & Placement Activity
 4. Temp Gross Margin Chart
 5. Direct Hire Revenue Chart

**Drill-through Functionality:**
The reports include drill-through functionality, allowing users to view detailed information by interacting with the visuals. This ease of interaction enables the client to obtain deeper insights and make informed business decisions.

# Step-by-Step Process for Report Generation:

**KPI Metric Dictionary:**
The client shared a KPI metric dictionary from Bullhorn, which provided detailed definitions of key performance indicators (KPIs).

**KPI Catalogue Creation:**
 1. We created a comprehensive KPI catalogue, which listed around 100 KPIs for six reports.
 2. Each KPI was thoroughly analysed, with logic defined in the catalogue by referencing Bullhorn's tables and columns that needed to be fetched

**Understanding and Logic Development:**
 1. We ensured a clear understanding of the KPIs by cross-referencing the metric dictionary and Bullhorn portal. Only the required columns were selected for data extraction.
 2. For each KPI, the associated logic was documented, detailing the table names and specific columns. This structured approach facilitated ease for both the development and ETL teams during the implementation phase.

**Client Review and Finalization:**
 1. After drafting the KPI logics, we conducted discussions with the client to review all the KPIs.
 2. Once the client had finalized the list, we moved forward with the report creation.

**UI Design and Approval:**
 1. Initially, the client was uncertain about the desired visualizations, so we created a draft UI for the report.
 2. After sharing the draft and making adjustments based on client feedback, the UI design was finalized through mutual agreement.

**Focusing on the First Report:**
 1. Although we had 100 KPIs in the catalogue, only specific KPIs were required for the initial Activity & Performance report.
 2. We created a separate sheet for this report, mapping the relevant KPIs to their corresponding visuals and ensuring a clear connection to the KPI catalogue.

**Data Fetching and Storage:**
 1. The required data was extracted from Bullhorn tables and stored in MySQL.
 2. Complex queries were written to perform the necessary calculations, which were then connected to Power BI for reporting.

**Final Report Development & testing:**
 1. The UI was built in Power BI as per the agreed design.
 2. We developed and optimized various DAX functions and Power BI queries to bring the report to life.
 3. After thorough testing, the report was moved to the UAT (User Acceptance Testing) environment for the client to review and finalize.
# Outcome: 
The new reporting system provides a much clearer picture of the client’s staffing operations, improving their ability to track and monitor key metrics. This helps streamline their staffing processes, enabling them to respond more effectively to business needs.
# Tools Used:
 1. Power BI: For data visualization and interactive reporting.
 2. MySQL: To store the transformed data.
 3. Python: For data extraction and ETL processes.
 4. AWS: For hosting and infrastructure needs.
# Delivered Reports:
Activity & Performance Report: Tracks employee and hiring metrics across various categories, including candidate activity, sales contacts, job placements, and revenue generation.
With this solution in place, the client now has enhanced reporting capabilities that help them track staffing performance across multiple industries and client organizations efficiently.
