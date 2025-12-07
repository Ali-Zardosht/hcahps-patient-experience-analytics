**HCAHPS Patient Experience Analytics**
Understanding patient satisfaction patterns through SQL-based ETL and Tableau data visualization

**Project Overview**
This project analyzes patient experience and satisfaction across U.S. hospitals using HCAHPS (Hospital Consumer Assessment of Healthcare Providers and Systems) survey data.

It follows a complete data engineering + analytics workflow, including:

SQL-based ETL & cleaning (MySQL)

Schema design & diagramming

Data transformation for Tableau

Interactive visual analytics

Insights for healthcare quality improvement

This project helps hospitals, administrators, and researchers understand:
 What drives patient satisfaction
 How states and hospitals differ
 Which communication domains matter most
 How survey volume and response rates influence ratings

**Tools & Technologies**
MySQL: MySQL Workbench	ETL, cleaning, transformation, schema building
Tableau: Visualization & exploratory analytics
Excel: CSV processing	, Pre-processing & validation
GitHub: Project documentation & version control

**Project Structure**
hcahps-patient-experience-analytics/
│
├── images/                       # Key project visualizations
│   ├── q1_avg_star_by_state.png
│   ├── q2_response_rates_hospitals.png
│   ├── q3_measure_groups_performance.png
│   ├── q4_states_high_satisfaction_bar.png
│   ├── q4_states_high_satisfaction_map.png
│   ├── q5_completed_vs_response_scatter.png
│   ├── q6_star_vs_response_scatter.png
│
├── sql/                          # ETL + cleaning SQL files
│   ├── create_schema.sql
│   ├── cleaning_transformations.sql
│   ├── loaded_tables_preview.sql
│
└── README.md                     # Project documentation

**Key Visual Insights**
1️⃣ Average Patient Survey Star Rating by State
Which states have the highest patient satisfaction?
Insight:
States such as Wisconsin, Nebraska, Idaho, Kansas, and South Dakota show the highest average satisfaction, while others trend lower due to population factors, hospital density, or regional care models.

2️⃣ Hospitals With the Highest Survey Response Counts (2023–2024)
Which hospitals collected the most patient feedback?
Insight:
Hospitals like AdventHealth Orlando and Orlando Health collected over 700,000–1,100,000 surveys, offering strong statistical reliability in patient satisfaction benchmarking.

3️⃣ HCAHPS Measure Group Performance
Which communication domains score highest nationally?
Insight:
Nurse Communication and Doctor Communication are top-performing domains.
Pain Management scores lowest, reflecting a known national trend after opioid-prescribing policy changes.

4️⃣ States With Consistently High Satisfaction
Where do patients report the best overall experience?
Bar Chart
Geographic Heatmap

Insight:
High-performing regions cluster in the Midwest and Mountain West, while larger urban states show more variability.

5️⃣ Do More Completed Surveys Mean Higher Response Rates?
Does survey volume influence response rate?
Insight:
There is no meaningful correlation.
Large hospitals gather more surveys simply due to size, not because patients respond at higher rates.

6️⃣ Correlation Between Star Ratings & Response Rates
Do happier patients respond more often?
Insight:
A positive moderate correlation exists:
Higher-rated hospitals tend to have better patient engagement and survey response rates — a meaningful behavioral signal.

**ETL & Data Preparation Summary (SQL Workflow)**
✔ Created relational schema
Tables:
Facility
Measure
Result
DatePeriod

✔ Cleaning Steps

Standardized string formats
Fixed missing or ambiguous Measure IDs
Converted percentages to numeric
Removed duplicate facility records
Aligned Measure–Result foreign keys
Created StarRating_Num (numeric rating)
Created calculated Linear Mean Value for Tableau

✔ Transformation for Tableau
Joined tables into a clean analytical dataset
Exported final fact table as .csv
Validated measures per hospital & date period
This clean pipeline ensured accurate visualization and statistical reliability.

**What I Learned**
Designing healthcare ETL workflows and relational schemas
Cleaning messy CMS and HCAHPS datasets using SQL
Building meaningful data visualizations in Tableau
Translating analytics into healthcare quality insights
Communicating complex metrics to non-technical audiences

**Contact**
If you'd like to discuss healthcare analytics, patient experience measurement, or data warehousing:

📧 ali.zardosht2025@yahoo.com

🔗 LinkedIn: https://www.linkedin.com/in/ali-zardosht
