# Patient Visit Analysis – Healthcare Clinic

## Project Overview
This project analyzes a synthetic dataset of 200 patient visits from a mid-sized healthcare clinic. The goal is to understand the demographic makeup of the patient population and identify the most common conditions treated.

**Key questions answered:**
- What is the age and gender distribution of visits?
- Which ICD codes appear most frequently?
- Who are the high-utilizer patients?
- How do common conditions vary by age group?

## Dataset
- **Source**: Synthetic patient visits data
- **Records**: 200 visits
- **Unique patient_ids**: 42
- **Fields**: visit_id, patient_id, visit_date, date_of_birth, patient_age, patient_sex, icd_code, cpt_code

### Important Data Limitation
Patient IDs are **not unique**. The same `patient_id` frequently appears with different dates of birth, ages, and even different sexes. This is likely due to data from multiple clinic branches being merged without proper patient matching.  

As a result, **all demographic analysis is performed at the visit level**, not the unique-patient level.

## Tools Used
- Excel (initial age calculation)
- Python (pandas, data cleaning & exploration)
- Tableau (visualization & dashboard)

<img width="1894" height="944" alt="PatientAnalysisDash" src="https://github.com/user-attachments/assets/390e4523-8e38-42c2-b4af-cb2ad779d128" />

<img width="640" height="480" alt="Age_Distributions" src="https://github.com/user-attachments/assets/d04e6f6a-03d8-4379-abb3-349f36e3f743" />

<img width="2000" height="800" alt="high_utilizers" src="https://github.com/user-attachments/assets/9ccb9622-7350-4fdb-9de2-1dbe55666ef7" />

<img width="2000" height="800" alt="icd_codes" src="https://github.com/user-attachments/assets/7871efc5-d8e3-45df-acb3-73c40a870e35" />

 
## Key Insights
| Insight | Finding |
|---------|---------|
| Age Distribution | 40–64 age group accounts for the most visits (98), followed by 18–39 (57) and 65+ (45) |
| Gender | Female visits: 117 · Male visits: 83 |
| Top ICD Code | **I10** (Essential hypertension) – 19 visits |
| Other common codes | N39.0, J45.909 (11 each), E11.9, M54.5, E78.5 (10 each) |
| High Utilizers | 20 patient_ids with 8–9 visits each |
| Age-specific patterns | 18–39: mental health & UTI codes more common<br>40–64: Asthma (J45.909) & diabetes-related<br>65+: Hypertension (I10) dominates |

## Files Included
- `patient_visits.csv` – Original data
- `patient_analysis.csv` – Cleaned & enriched data with age brackets
- `Patient_Visit_Analysis.ipynb` – Python analysis notebook
- `Patient Analysis.twbx` – Tableau workbook
- Visualizations (PNG)
- Project write-up (DOCX / PDF)

## How to Reproduce
1. Open the Jupyter notebook and run all cells.
2. Open the Tableau workbook (`.twbx`) to explore the interactive dashboard.

## Author
[Morris Mwangi Gitau]  
Data Analyst
