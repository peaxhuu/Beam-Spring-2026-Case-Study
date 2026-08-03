# Dental Insurance IBNP Reserving — Case Study

Actuarial case competition project estimating incurred-but-not-paid (IBNP)
claim reserves for a dental insurer, using three reserving methods applied
to a claims utilization and premium dataset.

## My Contribution
Led the **Projected Paid Lag method** implementation end-to-end.
Collaborated on the **Completion Factor** and **Bornhuetter-Ferguson**
methods as team approaches for comparison.

## Methods Implemented
- **Completion Factor** — projects ultimate claims from historical
  payment development patterns across mature service months
- **Bornhuetter-Ferguson (BF)** — blends an a priori expected loss ratio
  with actual paid claims; more robust for recent, less-mature periods
- **Projected Paid Lag** — estimates ultimate claims using the
  incremental (rather than cumulative) share of claims paid at each lag

## Key Result
Estimated an a priori expected loss ratio (ELR) of ~72% from mature
service months. Given rapid premium growth during the experience
period, the **Bornhuetter-Ferguson method** was recommended over pure
loss-development methods, since it remains reliable even when recent
months are still under-developed.

## Tools
R, RStudio, Quarto (`dplyr`, `tidyr`, `ggplot2`)

## Repo Structure
```
scripts/    Analysis code (Quarto document)
data/       Not committed — see data/README.md
output/     Generated charts/exports (gitignored by default)
```

## Data
The competition dataset is proprietary and is **not included** in this
repo. To reproduce the analysis, place the workbook at
`data/case_competition_data.xlsx` with sheets named `Utilization Data`
and `Premium Data`. See `data/README.md` for details.

## Note
This was completed as part of a case study competition
(Finalist, BEAM Case Study Competition, March 2026). Shared here for
portfolio purposes with methodology intact; underlying competition data
withheld per competition guidelines.
