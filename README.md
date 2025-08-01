---

### **Project Title: Public Health Disparity Analysis in India**

#### **Project Overview**

This project is an end-to-end data analysis workflow simulating a real-world scenario of a data analyst. It focuses on identifying and analyzing regional disparities in public health infrastructure, outcomes, and socio-economic factors in India. The analysis culminates in a focused case study comparing the public health landscapes of **Bihar** and **Kerala**, two states with vastly different socio-economic profiles.

This project demonstrates proficiency in the complete data analysis lifecycle, from handling messy, authentic data to generating and communicating compelling, data-backed insights.

#### **Key Questions Addressed**

* How do key public health outcomes (e.g., institutional births) correlate with socio-economic indicators (e.g., female school attendance)?
* What significant disparities exist in health infrastructure and service delivery (e.g., ANC registrations) between states?
* How can data from multiple, inconsistent sources be cleaned and integrated to support a comparative analysis?

#### **Methodology & Project Journey**

The project followed a standard data analysis methodology, with a strong emphasis on problem-solving and adapting to real-world data challenges.

1.  **Data Acquisition**: Sourced three distinct datasets from the Government of India's Open Government Data (OGD) platform:
    * **Health Management Information System (HMIS) Data**: Provided granular, district-level data on health infrastructure and service utilization.
    * **National Family Health Survey (NFHS) Factsheets**: Offered state-level data on key health outcomes and population characteristics.
    * **National Literacy Rate Data**: Provided socio-economic context for the analysis.

2.  **Data Cleaning & Preprocessing**: This was the most critical phase, involving significant data wrangling to prepare the data for analysis.
    * **Dataset Integration**: Combined data from multiple years and files into unified DataFrames.
    * **Handling Inconsistencies**: Addressed issues such as **`UnicodeDecodeError`** by specifying the correct encoding (`latin1`) and **`KeyError`** by programmatically identifying and selecting columns with inconsistent names.
    * **Data Transformation**: Converted datasets from a "wide" to a "long" format for time-series analysis and pivoted data for a clean, merged final DataFrame.
    * **Data Limitations**: Acknowledged and adapted to data limitations, such as a broken full-dataset download link and a fragmented reporting period across the HMIS files, which led to a focused case study.

3.  **Exploratory Data Analysis (EDA)**: Performed descriptive statistics and correlation analysis to identify key relationships.

4.  **Visualization & Communication**: Generated visualizations to effectively communicate the findings, including scatter plots to show correlations and bar charts to highlight disparities.

#### **Key Insights & Findings**

The analysis, though a focused case study, produced several compelling insights:

-   **Strong Correlation between Education and Health**: A near-perfect positive correlation ($r = 0.997$) was discovered between a state's **Female School Attendance Percentage** and its **Institutional Births Percentage**. This finding provides strong, data-backed evidence of the link between socio-economic factors and health outcomes.
-   **Service Delivery Disparity**: The data reveals a significant disparity in health service usage, with **Bihar** reporting a vastly higher number of **Antenatal Care (ANC) Registrations** than **Kerala**, despite having lower overall health outcomes. This is a crucial finding that merits further investigation into reporting methodologies and public health program effectiveness.

#### **Technologies Used**

* **Python**: The primary language for the entire analysis.
* **Pandas**: The core library for data manipulation, cleaning, and aggregation.
* **NumPy**: Used for numerical operations.
* **Matplotlib**: The primary library for creating static visualizations.
* **Jupyter Notebook**: The environment for a reproducible, step-by-step analysis and report.

#### **How to Run the Project**

1.  **Clone the repository**:
    `git clone https://github.com/harry3201/Health_Disparity_Analysis.git`
2.  **Install dependencies**:
    `pip install pandas numpy matplotlib`
3.  **Download the raw data**: The raw data files must be downloaded from the government portals mentioned in the notebook. Place them in the same directory as the notebook.
4.  **Run the Jupyter Notebook**: Open and run `Health_Disparities_Project.ipynb` to execute the complete analysis from start to finish.

---
