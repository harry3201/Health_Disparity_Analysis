#### **Public Health Disparity Analysis in India**
This project is an end-to-end data analysis workflow, simulating a real-world analysis scenario . The goal was to uncover regional disparities in public health and socio-economic factors in India by conducting a focused case study on the states of **Bihar** and **Kerala**. The project highlights the complete data analysis lifecycle, from raw data acquisition to generating compelling, data-backed insights.

---

#### **Project Goals**
* **Source Real-World Data**: Acquire and integrate authentic, inconsistent public datasets from the Government of India's Open Government Data (OGD) platform.
* **Data Wrangling**: Clean, transform, and prepare messy data, addressing common real-world challenges to create a unified and analysis-ready dataset.
* **Comparative Analysis**: Explore the relationships between health outcomes and socio-economic indicators, using a direct comparison of Bihar and Kerala.
* **Insight Generation**: Derive and communicate actionable insights that reveal disparities and potential areas for public health intervention.

---

#### **Key Challenges & Learnings**

This project's value lies in its realistic approach to data. Rather than using a clean dataset, I had to overcome several common data challenges:

* **Broken Data Links**: The main dataset for all states was unavailable, requiring me to manually download and combine individual state-wise files from different years.
* **Inconsistent Data Formats**: Data sources used different reporting periods and inconsistent column names, which I resolved by using programmatic methods to clean and unify the data.
* **Data Encoding Errors**: I encountered `UnicodeDecodeError` when loading CSV files, which I successfully resolved by identifying and specifying the correct file encoding (`latin1`).
* **Data Limitations**: The project's final scope was a focused case study due to fragmented reporting periods and missing columns across the raw datasets. This taught me to manage project expectations and adapt my analysis to the available data.

---

#### **Key Insights & Findings**

The final analysis, despite its focused scope, produced powerful and actionable insights:

-   **Education and Health Correlation**: A strong positive correlation ($r = 0.997$) was discovered between a state's **Female School Attendance Percentage** and its **Institutional Births Percentage**. This finding provides compelling evidence that improving female education can be a significant driver of better public health outcomes.
-   **Disparity in ANC Services**: A major disparity was identified in health service usage. **Bihar** reported a vastly higher number of **Antenatal Care (ANC) Registrations** than **Kerala**, despite having a lower institutional birth rate. This insight warrants further investigation into differences in data collection, service accessibility, and public health focus between the states.

---

#### **Technologies Used**
* **Python**
* **Pandas**: Performed Data manipulation, cleaning, and aggregation.
* **NumPy**: Used for numerical operations.
* **Matplotlib**: Created static visualizations.
* **Jupyter Notebook**
* **PowerBI**: Generated Dashboards for Insights 

---

#### **How to Run the Project**

1.  **Clone the repository**:
    `git clone https://github.com/harry3201/Health_Disparity_Analysis.git`
2.  **Install dependencies**:
    `pip install pandas numpy matplotlib`
3.  **Download raw data**: The raw data files used in this project must be downloaded from the government portals mentioned in the Jupyter Notebook and placed in the project directory.
4.  **Run the analysis**: Open and run `Health_Disparities_Project.ipynb` in a Jupyter environment to execute the complete analysis from start to finish.
