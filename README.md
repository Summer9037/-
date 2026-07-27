# E-commerce Advertising Click Analysis

> An end-to-end analysis of e-commerce advertising click behaviour, combining SQL and Python to identify practical CTR optimisation opportunities.

## Project overview

This project uses the Alibaba Tianchi advertising click-prediction dataset to examine factors associated with click-through rate (CTR). The analysis combines user attributes, advertising strategy, and product-price signals, turning exploratory findings into targeting and campaign recommendations.

## Highlights

- Worked with a large-scale public advertising-click dataset
- Used PostgreSQL and Python for joins, exploration, and visualisation
- Analysed CTR across user segments, ad campaigns, and price ranges
- Produced business-facing recommendations rather than charts alone

## Tech stack

- Python: Pandas, Matplotlib, Seaborn
- PostgreSQL
- Jupyter Notebook
- Git and GitHub

## Data source

Alibaba Tianchi public advertising click-prediction dataset, including:

- User behaviour logs: `raw_sample`
- Advertising metadata: `ad_feature`
- User profiles: `user_profile`

The original data is not included because of its size. Please obtain it from the original public source before reproducing the notebooks.

## Analysis workflow

1. **Data exploration and quality checks** — assess nulls, anomalies, duplicates, and the validity of core metrics.
2. **Overall CTR analysis** — calculate aggregate CTR, compare traffic placements, and inspect trends over time.
3. **User-segment analysis** — explore CTR differences by age, gender, and consumption level.
4. **Cross-dimensional analysis** — study age and consumption-level combinations while controlling for small samples.
5. **Advertising analysis** — compare advertisers, campaigns, and product-price bands.

## Key findings

- Overall CTR is approximately **5.14%**.
- User age groups 6 and 1 have the highest observed CTR and are promising targeting segments.
- CTR differs materially among advertisers and campaigns; the highest observed advertiser CTR exceeds 16%.
- Higher-priced products tend to have lower CTR, suggesting a trade-off between price and click attraction.

## Recommendations

1. Prioritise high-potential user segments, while validating performance on out-of-sample data.
2. Reuse patterns from strong campaigns and investigate underperforming ones.
3. Use lower-priced products for acquisition, and pair higher-priced products with richer content and more precise targeting.

## Repository structure

```text
ad_analysis_project/
├── notebooks/
│   ├── 01_database_exploration.ipynb
│   ├── 02_ctr_analysis.ipynb
│   ├── 03_user_analysis.ipynb
│   ├── 04_advanced_user_analysis.ipynb
│   ├── 05_advertiser_analysis.ipynb
│   └── 06_final_conclusion.ipynb
├── sql/
├── README.md
└── .gitignore
```

## Notes

This is an exploratory analytics project based on a public dataset. Findings should be revalidated before applying them to a live advertising system.
