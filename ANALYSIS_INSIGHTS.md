# Detailed Analysis Notes

This document expands the findings from the Excel workbook's analysis-ready `Healthcare_Data` sheet (10,000 rows).

## KPI definitions

- **Record count:** Number of rows in the analysis-ready table.
- **Average billing:** Arithmetic mean of the billing amount.
- **Average stay:** Arithmetic mean of the derived duration-of-stay field.
- **Condition frequency:** Count of records grouped by medical condition.

## Condition frequency

| Condition | Records | Share |
|---|---:|---:|
| Hypertension | 2,155 | 21.55% |
| Cancer | 1,647 | 16.47% |
| Obesity | 1,627 | 16.27% |
| Arthritis | 1,587 | 15.87% |
| Asthma | 1,550 | 15.50% |
| Diabetes | 1,434 | 14.34% |

## Average billing by condition

| Condition | Average billing |
|---|---:|
| Cancer | $39,676.54 |
| Diabetes | $30,070.07 |
| Asthma | $22,644.61 |
| Arthritis | $20,055.06 |
| Hypertension | $17,643.29 |
| Obesity | $12,535.69 |

The highest-to-lowest average billing ratio is approximately 3.16.

## Admission type comparison

| Admission type | Count | Average billing | Average stay |
|---|---:|---:|---:|
| Emergency | 3,587 | $24,279.06 | 15.62 days |
| Urgent | 3,336 | $22,731.21 | 15.42 days |
| Elective | 3,077 | $23,038.95 | 9.97 days |

Emergency stays average approximately 5.65 days longer than Elective stays.

## Insurance provider comparison

| Provider | Count | Average billing |
|---|---:|---:|
| Medicare | 2,428 | $22,942.94 |
| Cigna | 1,939 | $24,225.83 |
| Aetna | 1,921 | $24,131.55 |
| Blue Cross | 1,875 | $22,772.23 |
| UnitedHealthcare | 1,837 | $22,905.37 |

## Test results

| Result | Count | Share |
|---|---:|---:|
| Abnormal | 3,456 | 34.56% |
| Inconclusive | 3,277 | 32.77% |
| Normal | 3,267 | 32.67% |

## Age-segment comparison

| Segment | Count | Average billing | Average stay |
|---|---:|---:|---:|
| Young | 2,485 | $23,189.45 | 13.78 days |
| Middle | 4,444 | $23,135.87 | 13.76 days |
| Senior | 3,071 | $23,891.09 | 13.93 days |

## Quality checks and caveats

- 10,000 rows were analyzed.
- No exact duplicate rows were detected.
- No missing values were found in the main analysis fields checked.
- The recorded stay duration ranges from 0 to 30 days.
- Findings are descriptive and apply only to this synthetic sample. They should not be interpreted as clinical or causal conclusions.
