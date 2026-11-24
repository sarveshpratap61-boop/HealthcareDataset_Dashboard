# Healthcare Analytics Dashboard

An interactive healthcare data analytics project built with **Python, Pandas, Streamlit, and Plotly**. The project explores patient demographics, medical conditions, admissions, insurance providers, billing amounts, and test results through an interactive dashboard.

## Project Overview

This repository contains a healthcare dataset with **10,000 patient records and 17 columns**, along with a Streamlit dashboard and an Excel dashboard workbook.

The project is designed as a data analytics portfolio project to demonstrate data exploration, KPI reporting, data visualization, and interactive filtering.

## Dashboard Preview

The Streamlit dashboard includes:

- Total Patients
- Average Patient Age
- Total Billing Amount
- Average Length of Stay
- Patient distribution by gender
- Patient count by medical condition
- Admission trend by year
- Patient count by admission type
- Billing amount by insurance provider
- Test results distribution
- Blood type distribution
- Filtered patient records table
- Download option for filtered records in CSV format

## Dataset Description

**Dataset file:** `healthcare_dataset.csv`

**Dataset size:** 10,000 rows × 17 columns

| Column | Description |
|---|---|
| `Name` | Patient name |
| `Age` | Patient age |
| `Gender` | Patient gender |
| `Blood Type` | Patient blood group |
| `Medical Condition` | Recorded medical condition |
| `Date of Admission` | Patient admission date |
| `year-admission` | Year of admission |
| `Doctor` | Doctor associated with the record |
| `Hospital` | Hospital name |
| `Insurance Provider` | Patient's insurance provider |
| `Billing Amount` | Billing amount recorded for the patient |
| `Room Number` | Assigned room number |
| `Admission Type` | Admission category |
| `Discharge Date` | Patient discharge date |
| `discharge year` | Year of discharge |
| `Medication` | Medication recorded |
| `Test Results` | Recorded test result category |

## Tools and Technologies

- **Python** – application development
- **Pandas** – data loading, transformation, and aggregation
- **Streamlit** – interactive dashboard interface
- **Plotly Express** – interactive charts and visualizations
- **Excel** – supplementary dashboard and data review

## Repository Structure

```text
Healthcare-Analytics-Dashboard/
│
├── app.py
├── healthcare_dataset.csv
├── Healthcare_Analytics_Dashboard.xlsx
├── requirements.txt
├── README.md
└── .gitignore
```

## Run the Streamlit Dashboard Locally

### 1. Install Python

Install Python 3.9 or later.

### 2. Clone the repository

Replace `YOUR-USERNAME` with your GitHub username.

```bash
git clone https://github.com/YOUR-USERNAME/Healthcare-Analytics-Dashboard.git
```

### 3. Open the project folder

```bash
cd Healthcare-Analytics-Dashboard
```

### 4. Create a virtual environment (recommended)

**Windows:**

```bash
python -m venv venv
venv\Scripts\activate
```

**macOS / Linux:**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 5. Install the required libraries

```bash
pip install -r requirements.txt
```

### 6. Run the dashboard

```bash
streamlit run app.py
```

Streamlit will display a local URL in the terminal. Open that URL in your web browser. The default address is usually:

```text
http://localhost:8501
```

## Dashboard Filters

Use the sidebar filters to explore the records by:

- Admission Year
- Gender
- Medical Condition
- Admission Type
- Insurance Provider

The charts and patient table update according to the selected filters. You can also download the filtered records as a CSV file from the dashboard.

## Key Calculations

**Average Length of Stay**

The dashboard calculates length of stay using:

```python
Length of Stay = Discharge Date - Date of Admission
```

**Total Billing**

The total billing KPI is calculated by summing the `Billing Amount` values in the filtered records.

**Average Patient Age**

The average age KPI is calculated from the `Age` column in the filtered records.

## Excel Dashboard

The repository also includes `Healthcare_Analytics_Dashboard.xlsx`, which contains:

- A Dashboard worksheet with KPI summaries and charts
- A Healthcare Data worksheet containing the patient records

Open the workbook in Microsoft Excel to review the dashboard and dataset.

## Important Notes

- The source dataset does not specify a currency. The Streamlit dashboard currently displays billing values with a `$` symbol as a display convention. Confirm the intended currency before using these figures in a real-world report.
- Length of stay is calculated as the difference between discharge date and admission date, in days.
- This project is intended for learning and portfolio demonstration. It is not a clinical decision-support system.
- Review the dataset's privacy and usage permissions before publishing it publicly. Do not upload identifiable or confidential patient information without appropriate authorization.

## Future Enhancements

Potential next steps for this project:

- Add more advanced analysis and drill-down filters
- Connect the dashboard to a SQL database
- Add additional patient and hospital performance metrics
- Deploy the Streamlit dashboard online
- Add automated data validation and data-quality checks

## Author

**Sarvesh Pratap Srivastava**

Add your name and relevant profile links here before publishing the repository.

## GitHub Repository Description

Interactive Healthcare Analytics Dashboard built with Python, Pandas, Streamlit, and Plotly. Includes 10,000 patient records, interactive filters, KPI cards, visual analytics, and an Excel dashboard.
