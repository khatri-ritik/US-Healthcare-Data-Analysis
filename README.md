# 🏥 US Healthcare Data Analysis | Excel Portfolio Project

> An exploratory analysis of **10,000 synthetic healthcare records** using Microsoft Excel to understand patient demographics, medical conditions, admission patterns, billing, insurance providers, and length of stay.

<p align="left">
  <img src="https://img.shields.io/badge/Tool-Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white" alt="Microsoft Excel" />
  <img src="https://img.shields.io/badge/Analysis-Exploratory%20Data%20Analysis-2563EB?style=for-the-badge" alt="Exploratory Data Analysis" />
  <img src="https://img.shields.io/badge/Records-10%2C000-7C3AED?style=for-the-badge" alt="10,000 records" />
  <img src="https://img.shields.io/badge/Data-Synthetic-orange?style=for-the-badge" alt="Synthetic data" />
</p>

**Dataset notice:** All records are synthetic and intended for learning and portfolio demonstration. The findings are descriptive and should not be interpreted as clinical conclusions or evidence of causation.


## 📈 Interactive-style dashboard preview

The visual summary below brings together the headline KPIs, condition mix, average billing, admission patterns, insurance-provider volume, and age-segment distribution.

<p align="center">
  <img src="assets/healthcare_dashboard.svg" alt="US Healthcare analytics dashboard with KPI cards and charts" width="100%">
</p>


---

## 📌 Executive summary

This project uses Excel-based data preparation, PivotTables, PivotCharts, and descriptive analysis to explore 10,000 healthcare records covering **30 October 2018 to 30 October 2023**.

The analysis examines six medical-condition categories, three admission types, five insurance providers, demographic segments, billing amounts, and duration of stay. It highlights how record volume and average billing can tell different stories—for example, Hypertension is the most frequent condition, while Cancer has the highest average billing.

## 📊 Project at a glance

| KPI | Result |
|---|---:|
| Healthcare records | **10,000** |
| Analysis columns | **22** |
| Admission date range | **30 Oct 2018 – 30 Oct 2023** |
| Average patient age | **51.45 years** |
| Average billing amount | **$23,381.11** |
| Average length of stay | **13.82 days** |
| Total recorded billing | **$233.81 million** |
| Female / Male records | **5,075 / 4,925** |
| Missing values in analysis table | **0** |
| Exact duplicate rows | **0** |

## 🔍 Key business insights

<p align="center">
  <img src="assets/key_insights.svg" alt="Four headline healthcare analytics findings" width="100%">
</p>


### 1. Medical condition analysis

- **Hypertension** is the most frequent condition, with **2,155 records (21.6%)**.
- **Cancer** has the highest average billing at **$39,676.54** per record.
- Diabetes has the second-highest average billing at **$30,070.07**.
- Obesity has the lowest average billing among the six categories at **$12,535.69**.

**Business takeaway:** The most common condition is not necessarily the condition with the highest average billing. Volume and financial measures should be presented separately.

### 2. Admission type analysis

| Admission type | Records | Average billing | Average stay |
|---|---:|---:|---:|
| Emergency | 3,587 | $24,279.06 | 15.62 days |
| Urgent | 3,336 | $22,731.21 | 15.42 days |
| Elective | 3,077 | $23,038.95 | 9.97 days |

- Emergency admissions account for the largest share of records (**35.9%**).
- Emergency admissions have the highest average billing.
- Emergency and Urgent admissions have longer average stays than Elective admissions.

**Business takeaway:** Admission type is a useful dimension for monitoring differences in billing and length of stay.

### 3. Insurance provider analysis

| Provider | Records | Average billing |
|---|---:|---:|
| Medicare | 2,428 | $22,942.94 |
| Cigna | 1,939 | $24,225.83 |
| Aetna | 1,921 | $24,131.55 |
| Blue Cross | 1,875 | $22,772.23 |
| UnitedHealthcare | 1,837 | $22,905.37 |

- Medicare represents the largest record count (**24.3%**).
- Cigna has the highest average billing (**$24,225.83**), narrowly ahead of Aetna.

**Business takeaway:** Provider-level reporting should compare both record volume and average billing. Average billing does not represent insurer reimbursement or payment.

### 4. Patient demographic analysis

- Female records: **5,075 (50.75%)**.
- Male records: **4,925 (49.25%)**.
- Middle-age segment: **4,444 records**, the largest age group.
- Senior records have the highest average billing by age segment (**$23,891.09**).

**Business takeaway:** Demographic segmentation helps describe the composition of the dataset and compare group-level metrics.

### 5. Time-based analysis

- The dataset covers records from October 2018 to October 2023.
- Annual record volumes are relatively consistent across the complete calendar years.
- 2018 and 2023 are partial years, so their record counts should not be compared directly with full-year totals.

### 6. Relationship analysis

| Variable pair | Pearson correlation |
|---|---:|
| Age and billing amount | 0.013 |
| Age and duration of stay | 0.004 |
| Billing amount and duration of stay | -0.003 |

The correlations are close to zero, indicating little linear association in this synthetic sample. Correlation does not establish causation and does not rule out non-linear or subgroup patterns.

---

## 💡 Recommendations from the analysis

These are analytical recommendations for reporting and further investigation—not clinical recommendations.

1. **Monitor condition volume and billing separately:** A high-volume category may not have the highest average billing.
2. **Track admission patterns:** Compare average stay and average billing across Emergency, Urgent, and Elective admissions.
3. **Build an insurer comparison view:** Display record count alongside average billing to avoid misleading comparisons.
4. **Use demographic filters carefully:** Allow age and gender segmentation while clearly identifying the synthetic nature of the records.
5. **Add time filters:** Distinguish partial years from complete years in trend charts.
6. **Validate data before reporting:** Retain missing-value, duplicate, and consistency checks as part of the analysis workflow.

## 🧹 Data preparation and analysis workflow

1. Reviewed the raw dataset and workbook structure.
2. Prepared the analysis table and standardized relevant fields.
3. Used date, age-segment, demographic, and length-of-stay fields for analysis.
4. Checked the 10,000-row analysis table for missing values and exact duplicate rows.
5. Built PivotTable summaries for medical conditions, admission types, insurance providers, and demographics.
6. Compared average billing and length of stay across categories.
7. Interpreted the results and documented the analytical limitations.

## 🧰 Tools and skills demonstrated

| Area | Skills |
|---|---|
| Spreadsheet analysis | Microsoft Excel |
| Data preparation | Cleaning, standardization, validation |
| Data summarization | PivotTables |
| Data visualization | PivotCharts and chart interpretation |
| KPI reporting | Counts, averages, percentages, correlation |
| Analytical thinking | Segmentation, comparison, insight generation |
| Communication | Business takeaways and limitations |

## 📁 Project files

- **[Detailed Insights](INSIGHTS.md)** – Additional breakdowns, comparisons, data-quality checks, and methodology notes.
- **Excel workbook** – Source workbook and analysis sheets available in this repository.

## ⚠️ Interpretation, assumptions and limitations

- The dataset is entirely synthetic and does not represent real patients or actual healthcare-provider performance.
- The analysis is record-based. Repeated patient-name strings mean that the 10,000 records should not automatically be interpreted as 10,000 unique individuals.
- Average billing is not the same as cost, reimbursement, profit, or patient out-of-pocket expense.
- Differences between groups do not establish causation.
- Correlation measures only linear association and should be interpreted with care.
- This project is for analytics learning and portfolio demonstration, not medical, financial, or policy decision-making.

## 👨‍💻 About the author

I am building my Data Analytics portfolio after **four years of experience in AC compressor manufacturing**. I am developing practical skills in Excel, Power BI, SQL, and Python, with a focus on turning raw data into clear, useful insights.

**Author:** Ritik Khatri  
**GitHub:** [khatri-ritik](https://github.com/khatri-ritik)

## ✅ Conclusion

This project demonstrates how Microsoft Excel can be used to prepare, summarize, and analyze healthcare records. The analysis highlights differences in condition frequency, average billing, admission patterns, insurance-provider records, and patient demographics.

The key learning is to move beyond presenting numbers: validate the data, compare the right metrics, explain what the findings mean, and communicate limitations clearly.

---

*If you find this project useful, feel free to explore the repository and share feedback.*
