# Healthcare-Data-Analysis
This project analyze patient's health and diagnose trends in hospital charges, BMI, and chronic conditions using Excel and Pivot Tables & Charts.

**Project Overview and Objective:**
The objective of this project was to perform a comprehensive diagnostic analysis of patient healthcare data integrating demographic, medical examination, and hospitalization records to identify key factors driving high healthcare costs and contributing to poor patient outcomes. The project emphasizes rigorous data cleaning and transformation within the Excel environment to establish a reliable foundation for statistical analysis and dashboarding.

**Problem Statement:**
The project began with a fundamental data challenge: the information was fragmented across three separate tables, preventing any immediate cross-analysis. This forced us to first clean, merge, and transform the raw data to calculate essential diagnostic metrics. The primary challenge was to successfully integrate these datasets and then perform multi-dimensional analysis to answer critical questions about high hospital charges and the prevalence of chronic conditions (e.g., BMI, Diabetes Status).

**Attribute Details:**
The analysis utilized attributes from the integrated master sheet, covering three main categories:
Identifiers/Keys
Customer ID (Text): The unique ID used as the relational key for manually merging all three source tables.
Financial/Metric
Charges (Decimal): The core financial metric used to determine cost drivers and calculate all average costs.
Health Status
BMI (Decimal): Used to classify patients into Weight Status and analyze health profile severity.
Diabetes Status (Text): A primary diagnostic variable used to analyze its correlation with hospital charges.
Categorical & Segmentation
Smoker (Text): A key categorical variable used for risk segmentation (e.g., analyzing Cancer History distribution).
Hospital Tier (Text): Used for auditing cost variation across different facility levels as required by the assignment.
City Tier (Text): Used for auditing cost variation based on geographical location.

**Tools & Technologies:**

Tool: Microsoft Excel

Data Integration: Manual Key-Based Merging

Analysis: Pivot Tables and Quick Analysis (AI-driven features)

Visualization: Excel Charts and Slicers

**Data Pre-Processing:**
Data cleaning and transformation were executed strictly based on the requirements to ensure the dataset was reliable.
Missing Value: An initial task was performed to check and quantify all missing values (marked with '?') in the source tables.
Numerical Imputation: Missing values in the 'year' column were imputed using the calculated average of the existing 'year' values, rounded to the nearest integer.
Categorical Imputation: Missing values in the 'month' column were filled with the categorical value 'Sep'.
Missing values in 'smoker', 'hospital tier', and 'city tier' were filled using the most frequently occurring value (Mode) for each respective column.
Data Integration (Manual Merge): The three source files were manually consolidated into a single sheet and aligned records accurately.

**Analysis and Visualizations:**
The analysis was performed using a combination of Pivot Tables and AI-driven features as per the requirement.
Core Analysis: Pivot Tables were created to establish key cross-tabulations, such as Charges by Weight Status and Cancer History distribution among smokers vs non-smokers.
Summary Statistics (AI-Driven): Used Quick Analysis features to calculate overall statistics (Total customers count, Average costs, etc.) and generate basic visualizations.
Dashboard Creation: An interactive dashboard was built using the visualizations and incorporating Slicers for dynamic filtering.

**Insights and Conclusion:**

**Key Findings:**

Cost Drivers: Obese patients and those with Diabetes status were identified as having the highest average hospital charges.
Surgical Risk: Patients with higher Number of Major Surgeries has significantly increased average charges.
Risk Audit: Analysis of Smoker Status vs. Cancer History revealed similar rates of cancer history among both groups (around 17%), showing the risk is widespread in this specific dataset.

**Analysis Insights:**
The diagnostic analysis of the patient data yielded four critical insights for improving resource allocation and cost management:
Descriptive: The data clearly shows that Obese patients and those diagnosed with Diabetes are the high-cost groups, accounting for the highest total healthcare costs.
Diagnostic: Patients with a higher Number of Major Surgeries or those treated in Hospital Tier 1 facilities are the primary drivers of increased average charges, diagnosing where the most expensive care interventions are occurring.
Predictive: Given the strong correlation between poor health markers (BMI, Diabetes) and high costs, we can predict that a strategic focus on preventative care and management for these high-risk groups will effectively reduce the burden of future high-cost hospitalizations.
Prescriptive: To immediately manage costs, we recommend auditing the charges associated with Hospital Tier 1 facilities and the most frequent procedures, as this is the costliest segment of care identified in the dataset.

**Conclusion:**
The project successfully built a reliable master dataset by rigorously cleaning and manually integrating three fragmented healthcare records in Excel. The final dashboard delivers essential diagnostic insights on the major cost drivers and patient risk profiles, showcasing end-to-end proficiency in data preparation, statistical analysis, and visualization.
