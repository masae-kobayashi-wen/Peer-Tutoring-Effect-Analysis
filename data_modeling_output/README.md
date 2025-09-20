# Modeling Output

This folder contains statistical visualizations and model outputs from the tutoring effectiveness analysis.

## Visualizations (included)
- `ecdf_2025Q1.png` - Empirical Cumulative distribution with maximum gap of 43.65% at zero completions
- `boxplot_2025Q1.png` - Median and quartile comparison of tutored vs untutored students
- `violin_2025Q1.png` - Bimodal density distributions with embedded box plots
- `histogram_2025Q1.png` - Overlay density histogram showing engagement patterns

## Statistical Test Results (included)
- `descriptive_stats_2025Q1.csv` - Summary descriptive statistics by group (All/Tutored/Untutored)
- `histogram_table_2025Q1.csv` - Density values for completion count distributions
- `wilcoxon_2025Q1.csv` - Mann-Whitney U test results (p < 0.00001)
- `permutation_2025Q1.csv` - Permutation test for mean and median differences
- `bootstrap_2025Q1.csv` - Bootstrap confidence intervals for effect sizes
- `statistical_test_summary.csv` - Consolidated results from all statistical tests

## Model Outputs (included)
- `zinb_model_metrics_2025Q1.csv` - Key model metrics including coefficients, IRR values, and confidence intervals

## Files Not Included (Privacy)
- `BUS500-501_2025Q1_glm.csv` - Combined dataset with tutoring indicator prepared for GLM analysis
- `zinb_model_2025Q1.pkl` - Fitted Zero-Inflated Negative Binomial model object

## Key Findings
- **Tutoring Effect**: 2.16x improvement in completion rate (IRR: 2.16, 95% CI: [1.56, 3.01], p < 0.00001)
- **Zero Completions**: Reduced from 77% (untutored) to 33% (tutored)
- **Model Selection**: ZINB outperforms standard NB (AIC: 4923.57 vs 4946.51)