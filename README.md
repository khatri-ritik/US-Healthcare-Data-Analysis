# US Healthcare Data Analysis | Excel Portfolio Project

![Excel](https://img.shields.io/badge/Tool-Microsoft%20Excel-217346?logo=microsoft-excel&logoColor=white)
![Dataset](https://img.shields.io/badge/Records-10%2C000-blue)
![Status](https://img.shields.io/badge/Project-Completed-success)
![Data](https://img.shields.io/badge/Data-Synthetic-brightgreen)

An end-to-end exploratory analysis of **10,000 synthetic healthcare records** using Microsoft Excel. The project explores patient demographics, medical conditions, admission patterns, insurance providers, billing amounts, and length of hospital stay.

> **Dataset note:** The workbook owner confirms that the data is synthetic. It is not real patient data and should not be used to make clinical decisions.

## Dashboard preview

![Healthcare analysis dashboard](assets/healthcare_dashboard.svg)

![Key insights](assets/key_insights.svg)

## Executive KPI snapshot

| KPI | Result |
|---|---:|
| Healthcare records analyzed | **10,000** |
| Average patient age | **51.45 years** |
| Average billing amount | **$23,381.11** |
| Median billing amount | **$20,280.00** |
| Average length of stay | **13.82 days** |
| Female records | **5,075 (50.75%)** |
| Male records | **4,925 (49.25%)** |

## Key business insights

### 1. Patient and condition mix
- **Hypertension** is the most frequently recorded condition: **2,155 cases (21.55%)**.
- Cancer accounts for **1,647 records**, followed by Obesity (1,627), Arthritis (1,587), Asthma (1,550), and Diabetes (1,434).
- The dataset is relatively balanced by gender: 50.75% female and 49.25% male.

### 2. Billing patterns by medical condition
| Medical condition | Records | Average billing |
|---|---:|---:|
| Cancer | 1,647 | **$39,676.54** |
| Diabetes | 1,434 | $30,070.07 |
| Asthma | 1,550 | $22,644.61 |
| Arthritis | 1,587 | $20,055.06 |
| Hypertension | 2,155 | $17,643.29 |
| Obesity | 1,627 | **$12,535.69** |

Cancer has the highest average billing in this dataset, approximately **3.16×** the average billing for Obesity. This is a descriptive comparison, not evidence that the condition itself causes higher costs.

### 3. Admission type and length of stay
| Admission type | Records | Average billing | Average stay |
|---|---:|---:|---:|
| Emergency | 3,587 | **$24,279.06** | **15.62 days** |
| Urgent | 3,336 | $22,731.21 | 15.42 days |
| Elective | 3,077 | $23,038.95 | 9.97 days |

Emergency admissions have the highest average billing, while Emergency and Urgent admissions have longer average stays than Elective admissions. Emergency average stay is about **5.65 days longer** than Elective.

### 4. Insurance provider snapshot
| Insurance provider | Records | Average billing |
|---|---:|---:|
| Medicare | 2,428 | $22,942.94 |
| Cigna | 1,939 | **$24,225.83** |
| Aetna | 1,921 | $24,131.55 |
| Blue Cross | 1,875 | $22,772.23 |
| UnitedHealthcare | 1,837 | $22,905.37 |

Medicare has the largest record count, while Cigna has the highest average billing among the providers in this dataset.

### 5. Test-result distribution
| Test result | Records | Share |
|---|---:|---:|
| Abnormal | 3,456 | 34.56% |
| Inconclusive | 3,277 | 32.77% |
| Normal | 3,267 | 32.67% |

The three result categories are relatively evenly represented. The workbook does not provide clinical interpretation or outcome follow-up, so these counts should be treated only as descriptive.

### 6. Age segment
| Age segment | Records | Average billing |
|---|---:|---:|
| Young | 2,485 | $23,189.45 |
| Middle | 4,444 | $23,135.87 |
| Senior | 3,071 | $23,891.09 |

Senior records show a modestly higher average billing in this sample. The difference is descriptive and does not establish an age-related causal effect.

## Data preparation and Excel workflow

The workbook contains a raw-data sheet, a cleaned/analysis-ready healthcare table, PivotTable summaries, advanced analysis, dashboard insights, and notes documenting data preparation.

The documented preparation work includes:
- Preserving a backup of the raw data.
- Removing unnecessary columns.
- Standardizing gender values (for example, `M` to `Male`).
- Standardizing blood-group labels and positive/negative notation.
- Standardizing admission labels (for example, `Emer` to `Emergency`).
- Creating analysis fields such as age bucket, demographic segment, duration of stay, year, month, day, month name, and week of stay.

Additional validation from the analysis-ready sheet:
- **10,000 rows** and no exact duplicate rows detected.
- No missing values in the main analysis fields reviewed.
- Admission categories were normalized to Emergency, Urgent, and Elective.

## Workbook structure

- `Healthcare_Data` — cleaned, analysis-ready records.
- `Main Sheet` — additional derived fields, including week-of-stay grouping.
- `Pivot Insights`, `Sample Sale Analysis`, `Advance Ananlysis`, and `Insights` — summary and pivot-based analysis areas.
- `Notes` — data-cleaning notes, category mappings, and analysis hypotheses.

## Skills demonstrated

- Excel data cleaning and standardization
- PivotTables and summary analysis
- KPI development
- Descriptive statistics and segmentation
- Billing and operational trend analysis
- Dashboard storytelling and business communication

## Repository contents

- [Dashboard preview](assets/healthcare_dashboard.svg)
- [Key insights graphic](assets/key_insights.svg)
- [Detailed analysis notes](ANALYSIS_INSIGHTS.md)

## Limitations

This is a synthetic dataset and the analysis is exploratory. Results describe patterns in this sample only. They do not establish causation, clinical effectiveness, provider quality, or real-world healthcare costs. The source workbook also contains a minimum recorded stay of zero days; interpret stay-duration averages with that data characteristic in mind.

## About the author

**Ritik Khatri** — transitioning into Data Analytics after four years of experience in AC compressor manufacturing. Currently building practical skills in Excel, Power BI, SQL, and Python.

- GitHub: [@khatri-ritik](https://github.com/khatri-ritik)

---
If you find this project useful, feel free to ⭐ the repository.
