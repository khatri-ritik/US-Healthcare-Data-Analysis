# US Healthcare Data Analysis | Excel Portfolio Project

An end-to-end exploratory data analysis project using **Microsoft Excel** to examine 10,000 synthetic healthcare records. The analysis focuses on patient demographics, medical conditions, admission patterns, billing, insurance, and length of stay.

> **Dataset note:** All records in this project are synthetic and are used for learning and portfolio demonstration. Findings are descriptive, not clinical conclusions or evidence of causation.

## 📌 Project at a glance

| KPI | Result |
|---|---:|
| Healthcare records | **10,000** |
| Admission date range | **Oct 2018 – Oct 2023** |
| Average patient age | **51.45 years** |
| Average billing amount | **$23,381.11** |
| Average length of stay | **13.82 days** |
| Female / Male records | **5,075 / 4,925** |
| Total recorded billing | **$233.81 million** |

## 🔎 Key insights

1. **Hypertension is the most common condition:** 2,155 records (21.6% of the dataset).
2. **Cancer has the highest average billing:** $39,676.54 per record, around 2.25× the hypertension average ($17,643.29).
3. **Emergency admissions have the highest average billing:** $24,279.06, compared with $23,038.95 for Elective and $22,731.21 for Urgent admissions.
4. **Emergency stays are longer:** 15.62 days on average, compared with 15.42 days for Urgent and 9.97 days for Elective admissions.
5. **Medicare has the largest record count:** 2,428 (24.3%). Cigna has the highest average billing among providers at $24,225.83, narrowly above Aetna at $24,131.55.
6. **Senior records have the highest average billing by age segment:** $23,891.09, versus $23,135.87 for Middle and $23,189.45 for Young.
7. **Gender mix is broadly balanced:** Female records represent 50.75% and Male records 49.25%.
8. **Age and billing are nearly uncorrelated in this dataset:** Pearson correlation is approximately 0.013. This is a descriptive pattern, not a causal finding.

## 📊 Explore the detailed analysis

See [INSIGHTS.md](INSIGHTS.md) for additional breakdowns, comparisons, interpretation notes, and portfolio-ready observations.

## 🧰 Tools & skills demonstrated

- Microsoft Excel
- Data cleaning and standardization
- PivotTables and PivotCharts
- KPI design and dashboard reporting
- Descriptive statistics and segmentation
- Exploratory data analysis and business storytelling

## 🧹 Analysis workflow

1. Reviewed the raw data and working sheets.
2. Standardized categorical values and prepared date, age-band, demographic-segment, and length-of-stay fields.
3. Checked the 10,000-row analysis table for missing values and exact duplicate rows.
4. Built PivotTable summaries for conditions, admission types, insurance providers, demographics, and billing.
5. Compared average billing and stay duration across groups.
6. Converted the results into concise operational observations.

## 💡 Potential business questions

- Which conditions account for the largest share of admissions?
- Which admission types are associated with higher average billing and longer stays?
- How do billing averages vary by condition and insurance provider?
- How is the patient population distributed by age and gender?
- Which patterns could be monitored in a healthcare operations dashboard?

## ⚠️ Interpretation & limitations

- The dataset is synthetic; it does not represent real patients or actual healthcare provider performance.
- Average billing is not the same as cost, reimbursement, profit, or patient out-of-pocket expense.
- Group differences do not establish that a condition, admission type, insurer, age, or gender caused a billing or stay outcome.
- The dataset contains repeated patient-name values; this analysis treats each row as a record and does not assume that each row represents a unique individual.
- This project is for data analytics practice, not medical, financial, or policy decision-making.

## 👨‍💻 About

I am building my Data Analytics portfolio after four years of experience in AC compressor manufacturing. I am developing practical skills in Excel, Power BI, SQL, and Python, with a focus on turning raw operational data into clear, useful insights.

**Author:** Ritik Khatri  
**GitHub:** [khatri-ritik](https://github.com/khatri-ritik)

---
*If you find this project useful, feel free to explore the repository and share feedback.*
