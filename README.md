# Infosys722--Assignment-4-BDAS
A reproducible pipeline for large-scale exploratory data analysis (EDA) and (optional) MLlib modeling on the Chicago Crime Dataset (2017). The project emphasizes PySpark DataFrames for scalable aggregation, window-based rankings for hotspot exploration, and baseline classification/regression models.  
BDAS Crime Analysis (Chicago 2017) — PySpark + Google Colab

A reproducible pipeline for large-scale exploratory data analysis (EDA) and (optional) MLlib modeling on the Chicago Crime Dataset (2017). The project emphasizes PySpark DataFrames for scalable aggregation, window-based rankings for hotspot exploration, and baseline classification/regression models.

✨ What’s inside

Colab-ready notebooks to ingest the Kaggle CSV and generate Figures 5–11 (top categories, arrest rates, month/weekday/hour trends, domestic vs non-domestic, hexbin map).

PySpark DataFrame patterns: selections, filters, derived time fields, groupBy/aggregations, window functions (Top-K per period).

Optional MLlib baselines:

Hotspot classification (next-month Top-K% by district/beat) with AUC and HitRate@K.

Monthly count forecasting (per district/beat) with MAE vs seasonal naïve (same month last year).

Time-aware evaluation: final hold-out window + rolling CV.

Environment

Python 3.11 (Colab)

PySpark 3.5.1

pandas, numpy, matplotlib, seaborn (for lightweight visuals)

Objectives & Metrics (summary)

EDA outputs: interpretable trends and window-based Top-K rankings.

Hotspot classification (MLlib): target is “next-month Top-K% unit”; report AUC and HitRate@K (K ≈ 10%).

Count forecasting (MLlib): monthly incidents per unit; report MAE/RMSE vs seasonal naïve (lag-12).

Robustness: time-ordered splits + rolling CV; control leakage (only use past data to predict future).

🔒 Ethics & governance

Dataset is public, anonymized, and intended for academic use. We avoid re-identification, document class imbalance and bias, and report limitations.

🙏 Acknowledgements

University of Auckland—Infosys 722. Thanks to the City of Chicago and Kaggle for making the dataset publicly available.
