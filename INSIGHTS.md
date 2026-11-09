# Detailed Insights | US Healthcare Data Analysis

**Source:** Attached Excel workbook, primarily the `Healthcare_Data` analysis table.  
**Sample:** 10,000 synthetic records.  
**Period:** 30 October 2018 to 30 October 2023.

## 1. Dataset quality snapshot

| Check | Result |
|---|---:|
| Rows in analysis table | 10,000 |
| Columns | 22 |
| Missing values in analysis table | 0 |
| Exact duplicate rows | 0 |
| Distinct patient-name strings | 9,378 |

The name count is not treated as a unique-patient count: repeated name strings occur, and synthetic records may reuse names. All analysis below is record-based.

## 2. Condition mix and average billing

| Medical condition | Records | Share | Average billing |
|---|---:|---:|---:|
| Hypertension | 2,155 | 21.6% | $17,643.29 |
| Cancer | 1,647 | 16.5% | $39,676.54 |
| Obesity | 1,627 | 16.3% | $12,535.69 |
| Arthritis | 1,587 | 15.9% | $20,055.06 |
| Asthma | 1,550 | 15.5% | $22,644.61 |
| Diabetes | 1,434 | 14.3% | $30,070.07 |

**Observation:** Hypertension is the largest category by record count, while Cancer has the highest average billing. These are two different measures and should not be conflated.

## 3. Admission type: volume, billing and stay

| Admission type | Records | Share | Average billing | Average stay |
|---|---:|---:|---:|---:|
| Emergency | 3,587 | 35.9% | $24,279.06 | 15.62 days |
| Urgent | 3,336 | 33.4% | $22,731.21 | 15.42 days |
| Elective | 3,077 | 30.8% | $23,038.95 | 9.97 days |

**Observation:** Emergency is the largest admission group and has the highest average billing. Emergency and Urgent stays are both around 15–16 days, while Elective stays average about 10 days.

## 4. Insurance provider comparison

| Provider | Records | Average billing |
|---|---:|---:|
| Medicare | 2,428 | $22,942.94 |
| Cigna | 1,939 | $24,225.83 |
| Aetna | 1,921 | $24,131.55 |
| Blue Cross | 1,875 | $22,772.23 |
| UnitedHealthcare | 1,837 | $22,905.37 |

**Observation:** Medicare accounts for the most records (24.3%). Cigna has the highest average billing in this sample, followed closely by Aetna. This does not indicate differences in insurer payment or reimbursement.

## 5. Demographic patterns

| Age segment | Records | Average billing | Average stay |
|---|---:|---:|---:|
| Young | 2,485 | $23,189.45 | 13.78 days |
| Middle | 4,444 | $23,135.87 | 13.76 days |
| Senior | 3,071 | $23,891.09 | 13.93 days |

Female records: 5,075 (50.75%). Male records: 4,925 (49.25%).

The Senior segment has a modestly higher average billing in this dataset. Average stays are very similar across all three age segments.

### Condition distribution by gender

| Condition | Female records | Male records |
|---|---:|---:|
| Arthritis | 821 | 766 |
| Asthma | 742 | 808 |
| Cancer | 836 | 811 |
| Diabetes | 825 | 609 |
| Hypertension | 836 | 1,319 |
| Obesity | 1,015 | 612 |

Hypertension records skew male in this synthetic sample, while Obesity records skew female. These patterns should not be generalized to real populations.

## 6. Yearly record volume

| Year | Records | Average billing |
|---|---:|---:|
| 2018* | 303 | $23,435.58 |
| 2019 | 1,973 | $23,274.34 |
| 2020 | 2,044 | $23,883.21 |
| 2021 | 2,063 | $23,083.63 |
| 2022 | 2,001 | $23,644.83 |
| 2023* | 1,616 | $22,919.43 |

*2018 and 2023 are partial years in the dataset date range. Do not compare their raw record counts directly with full years.*

## 7. Statistical relationship check

Pearson correlation coefficients calculated from the 10,000 records:

| Variable pair | Correlation |
|---|---:|
| Age and billing amount | 0.013 |
| Age and duration of stay | 0.004 |
| Billing amount and duration of stay | -0.003 |

These values are close to zero, indicating little linear association in this synthetic sample. Correlation does not establish causation and does not rule out non-linear or subgroup relationships.

## 8. Portfolio takeaways

- Separate volume metrics (record count) from financial metrics (average billing).
- Use admission type as a useful dashboard dimension for comparing average stay and billing.
- Show condition-level averages alongside record counts to avoid misleading rankings.
- Add date filters and clearly flag partial years in time-series visuals.
- Include a data-quality section and an interpretation caveat in analytical deliverables.

## Method notes

- Currency values are displayed in USD as represented by the workbook's billing field.
- Percentages are calculated using 10,000 records as the denominator.
- Averages are arithmetic means; they can be affected by extreme values.
- All results are descriptive summaries of synthetic records, not clinical conclusions.
