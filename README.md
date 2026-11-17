<img width="1672" height="941" alt="Secure Life Hospistal - introduction image" src="https://github.com/user-attachments/assets/0cdefbfb-1682-4ad4-85db-f0f46d9fbbba" />

## SECURE-LIFE-HOSPITAL-ANALYTICS-DASHBOARD


HOSPITAL OPERATIONS AND REVENUE PERFORMANCE DASHBOARD 
Patient Admissions | Billing | Insurance | Payment Status

## Introduction
Secure Life General Hospital has noticed changes in patient admissions, outstanding medical bills and insurance coverage across its departments, but it has no single report that brings these together. This project turns the hospital’s raw patient, billing and insurance records into a Microsoft Excel analysis and an interactive dashboard that management can use to monitor operations, track payments and make better decisions.
The analysis covers 1,000 patient visits recorded between January 2024 and December 2025. It answers ten management questions about visit volumes, billing, length of stay, payment status, insurance coverage, patient age and trends over time, and it points out the areas that need management attention.
Tools used: Microsoft Excel (COUNTIFS, SUMIFS, AVERAGEIFS and date formulas, helper columns, charts, and Department, Year and Diagnosis filters on the dashboard).


## About the Dataset
The dataset has 1,000 rows and 11 columns. Each row is one patient visit, not necessarily one unique patient, so a patient could appear more than once. In this file every Patient ID is unique (PAT-3001 to PAT-4000), which means repeat visits cannot be identified.
Column
Description
Patient ID
Unique ID for each patient visit or record
Patient Name
Name of the patient who received care
Age
Patient age in years at the time of the visit
Gender
Patient gender as recorded
Admission Date
Date the patient was admitted
Discharge Date
Date the patient was discharged
Department
Cardiology, Emergency, General, Neurology, Orthopedics or Pediatrics
Diagnosis
Medical condition recorded (38 different diagnoses)
Total Bill Amount
Total amount the hospital charged for treatment and services
Insurance Coverage (%)
Percentage of the bill covered by the patient’s insurance
Payment Status
Paid, Pending or Partially Paid


## Columns added during analysis
Length of Stay (days): discharge date minus admission date.
Age Group: Under 18, Btw 18 & 35, Btw 36 & 50, Btw 51 & 65 and 66 & Above.
Admission Month and Admission Year: used for the admission trend and the Year filter.
Insurance Covered ($) and Patient Share ($): bill multiplied by coverage %, and the remainder of the bill.


## Data quality checks
No missing values and no discharge dates earlier than admission dates were found.
The dataset has no “amount paid” column, so the exact outstanding balance cannot be calculated. It is shown as a range instead (see Insights, section 6).

## Problem Statement
Management has observed a change in patient admissions, outstanding medical bills and variations in insurance coverage across departments. The hospital lacks a consolidated report showing its operational and financial performance. As the data analyst, the task was to transform the raw data into insights and a dashboard that helps management monitor performance and make informed decisions. The analysis aims to answer these questions:
How many patient visits has the hospital recorded?
Which departments receive the highest number of patients?
Which departments generate the highest total bills?
What is the average length of stay across departments?
What proportion of bills is paid, pending or partially paid?
How much has the hospital billed, and how much remains outstanding?
How does insurance coverage vary across departments and diagnoses?
Which age groups account for the most patient visits?
How do admissions and billing change over time?
Which areas may need management attention?


## Visualization
The dashboard has five KPI cards (No. of Patients, Total Bill Amt., Avg. Stay Length, Paid Amount and Avg. Insurance %) and five charts: admission trend over time, patients by department, patients by age group, payment status (%) and patients by gender. In the Excel file, the Department, Year and Diagnosis dropdown filters update every KPI and chart.


## Insights
1. Patient visits
1,000 patient visits were recorded across two years: 508 in 2024 and 492 in 2025.
2. Departments with the most patients
General (252 visits, 25.2%) is the busiest department, followed by Emergency (190) and Orthopedics (159). Pediatrics (153) and Cardiology (152) are almost level, and Neurology is the smallest with 94 visits.
3. Departments with the highest bills
Orthopedics generated $2.55M (31.7% of all billing) and Cardiology $2.10M (26.0%). Together they bring in 57.7% of billing from only 31.1% of visits.
Average bill per visit shows the gap clearly: Orthopedics $16,062, Cardiology $13,786 and Neurology $12,929, against $3,941 for General, $3,745 for Pediatrics and $3,276 for Emergency.
Carpal Tunnel ($589,740), Atrial Fibrillation ($546,653) and Knee Replacement ($494,615) are the three diagnoses with the highest total billing. The top 10 diagnoses (out of 38) make up 52.0% of all billing.
4. Average length of stay
The average stay is 4.8 days. Orthopedics has the longest at 8.4 days, then Neurology (6.9) and Cardiology (6.5). General averages 3.9 days, Pediatrics 3.0 and Emergency 2.0.
101 visits lasted 10 days or more, and the longest stay was 14 days. Long stays and high bills sit in the same departments.
5. Payment status
Paid: 564 visits (56.4%). Pending: 257 (25.7%). Partially Paid: 179 (17.9%). By value, the split is almost identical: 56.7% paid, 25.9% pending and 17.4% partially paid.
Paid Amount: $4,568,527 of the $8,053,143 billed. This is why the dashboard donut chart reads 57% Paid, 17% Partially Paid and 26% Pending (by bill amount).
Nearly 44% of visits (436) are not fully settled. The share is highest in General (46.8%) and Pediatrics (46.4%) and lowest in Emergency (37.9%).
6. Amount billed and outstanding
Total billed: $8,053,143 (average $8,053 per visit). Insurance covers about $6.06M of this and patients are responsible for about $1.99M.
Outstanding: between $2.08M and $3.48M. The lower figure counts only Pending bills ($2,082,786). The upper figure adds the full value of Partially Paid bills ($1,401,830), because the data does not show how much of those was paid.
Even in the best case, patients’ own share on unsettled bills is up to about $1.03M.
Orthopedics ($687K) and Cardiology ($525K) hold the largest Pending balances.
7. Insurance coverage
Average coverage is about 75% (74.9% unrounded) and is very even across departments, from 73.9% (General) to 76.3% (Cardiology).
Coverage varies much more by diagnosis. It is lowest for Asthma (61.5%), Arrhythmia (63.5%) and Epilepsy (67.9%), and highest for Coronary Artery Disease (82.9%), Stroke (82.2%) and RSV (80.8%).
44 visits had no insurance coverage at all. They were billed $345,195 in total, and 32 of them (73%) are not fully paid.
8. Age groups
The 51-65 group has the most visits (235), just ahead of 66 & Above (232), then 36-50 (210), 18-35 (170) and Under 18 (153). Patients aged 51 and over account for 46.7% of visits.
The 51-65 group also brings the most billing ($2.36M, average $10,028 per visit). Under 18 patients bring the least ($573K, average $3,745).
Gender is almost evenly split (512 female, 488 male: 51.2% and 48.8%) with similar average bills ($7,996 and $8,113).
9. Admissions and billing over time
Monthly admissions move between 29 and 57 with no steady upward or downward trend. The peak was November 2025 (57 admissions, $510K billed). The lowest months were June and August 2025 (29 each), and June 2025 had the lowest billing ($191K).
2025 recorded 3.1% fewer visits than 2024 (492 against 508) and 5.1% less billing ($3.92M against $4.13M).


Department summary
Department
Visits
Total Billed
Avg Stay (days)
Avg Insurance
Not fully paid
General
252
$993,027
3.9
73.9%
46.8%
Emergency
190
$622,525
2.0
76.2%
37.9%
Orthopedics
159
$2,553,862
8.4
74.5%
43.4%
Pediatrics
153
$572,988
3.0
74.0%
46.4%
Cardiology
152
$2,095,438
6.5
76.3%
43.4%
Neurology
94
$1,215,303
6.9
74.6%
42.6%
Hospital
1,000
$8,053,143
4.8
74.9%
43.6%

 

10. Areas needing management attention
Unpaid high-value bills. 85 visits billed $20,000 or more make up 27.4% of billing, and 35 of them (about $892K) are not fully paid.
Orthopedics and Cardiology. They carry the largest revenue, the longest stays and the biggest Pending balances, so delays in collection or discharge here affect the hospital most.
General and Pediatrics. They have the highest share of unsettled visits (46.8% and 46.4%) even though their bills are small.
Uninsured and low-coverage visits. Zero-coverage visits and low-coverage diagnoses such as Asthma and Arrhythmia are likely to produce unpaid patient balances.
Volume pressure. General and Emergency handle 44.2% of all visits with short stays, so they need steady staffing and fast patient turnover.



## Recommendations
Verify insurance before admission. Check coverage and obtain pre-authorisation for planned procedures such as knee replacement, spinal and hip surgery, and counsel patients with low or no coverage on payment plans before discharge.
Offer instalment plans for large patient shares. Bills of $20,000 and above are the biggest collection risk and may be easier to recover in stages.
Manage bed capacity in Orthopedics, Neurology and Cardiology. Review discharge planning to shorten stays above 10 days where it is clinically safe, which frees beds for more high-value cases.
Plan staffing around demand. Keep General and Emergency resourced for the highest volumes, and investigate what drove the November 2025 spike and the mid-2025 dips before setting next year’s staffing and budget.
Strengthen services for patients aged 51 and over. They are the largest and highest-billing group, so chronic-care and cardiology pathways for this group deserve priority.


## Conclusion
The hospital recorded 1,000 visits and $8.05M in billing over two years. Volume is highest in General and Emergency, but value is concentrated in Orthopedics and Cardiology, which earn 57.7% of billing from less than a third of visits and also keep patients the longest. Insurance coverage averages about 75% and is similar across departments, though some diagnoses and 44 uninsured visits are exposed.
The biggest concern is payment: about 44% of visits are not fully paid, leaving between $2.08M and $3.48M still to collect. Focusing on collections for high-value bills, insurance verification, discharge planning and better payment data would improve cash flow and give management a clearer view. The Excel dashboard can be refreshed with new data to keep monitoring these measures.


