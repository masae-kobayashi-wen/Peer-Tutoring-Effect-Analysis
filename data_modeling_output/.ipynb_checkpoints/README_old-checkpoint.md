# Modeling Output

This folder contains statistical visualizations and model outputs from the tutoring effectiveness analysis.

## Visualizations (included)
- `ecdf_2025Q1.png` - Empirical cumulative distribution showing 43.65% gap at zero completions
- `boxplot_2025Q1.png` - Median and quartile comparison of tutored vs untutored students
- `violin_2025Q1.png` - Density distributions with embedded box plots
- `histogram_2025Q1.png` - Overlaid density histograms showing engagement patterns

## Model Output (included)
- `zinb_model_metrics_2025Q1.csv` - Key model metrics including IRR and confidence intervals

## Files Not Included (privacy)
- `BUS500-501_2025Q1_glm.csv` - Combined dataset prepared for GLM analysis
- `zinb_model_2025Q1.pkl` - Fitted model object

## Key Finding
Tutoring results in a 2.16x improvement in student competency completion (p < 0.00001).