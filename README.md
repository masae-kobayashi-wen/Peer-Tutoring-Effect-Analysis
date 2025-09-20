# Peer Tutoring Effectiveness Analysis

## Project Overview
Statistical analysis demonstrating the impact of peer tutoring on student engagement in Calbright College's Data Analysis Program. Using advanced statistical modeling (Zero-Inflated Negative Binomial regression), this project shows that tutored students complete 2.16x more competencies than untutored students.

## Key Findings
- **2.16x improvement** in competency completion for tutored students (p < 0.00001)
- **44% reduction** in student disengagement (77% → 33% zero completions)
- **Clear ROI** for expanding tutoring programs

<p align="center">
  <img src="data_modeling_output/histogram_2025Q1.png" width="650">
</p>
<p align="center"><i>Density distribution showing dramatic reduction in zero-completion students with tutoring</i></p>

## Repository Contents

### Notebooks
1. **[DA_2025Q1_1a_post_tutor_form_wrangling.ipynb](notebooks/DA_2025Q1_1a_post_tutor_form_wrangling.ipynb)** 
   - Processes 449 tutoring session records
   - Identifies 137 unique tutored students
   - Handles data validation and manual email correction

2. **[DA_2025Q1_1b_gradebook_wrangling.ipynb](notebooks/DA_2025Q1_1b_gradebook_wrangling.ipynb)** 
   - Processes gradebook data for 2,558 students
   - Calculates quarterly progress metrics
   - Segments students by tutoring status

3. **[DA_2025Q1_2_statistical_modeling.ipynb](notebooks/DA_2025Q1_2_statistical_modeling.ipynb)** 
   - Performs statistical analysis including ZINB regression
   - Validates tutoring effectiveness with multiple methods
   - Generates visualizations and model metrics

### Key Visualizations
- [ECDF Analysis](data_modeling_output/ecdf_2025Q1.png) - Empirical cumulative distribution showing 43.65% gap in student engagement
- [Distribution Comparison](data_modeling_output/histogram_2025Q1.png) - Density histogram comparing progress distribution by tutoring status (shown above)
- [Model Metrics](data_modeling_output/zinb_model_metrics_2025Q1.csv) - Statistical model results including IRR, confidence intervals, and p-values

### Presentation
- [Executive Summary (PDF)](presentations/Calbright_Tutoring_Impact_Analysis_2025_MKW.pdf) - Stakeholder presentation with key findings and recommendations
- [Executive Summary (Google Slides)](https://docs.google.com/presentation/d/1XuSMRpGwxlzaQ8unsDDhAwWEUM7NEmPTf7Ub73tAdzI/edit?usp=sharing) - Includes detailed speaker notes

## Technical Skills Demonstrated
- **Data Wrangling**: Complex data cleaning, validation, and transformation
- **Statistical Analysis**: Zero-Inflated Negative Binomial (ZINB) regression, hypothesis testing
- **Python Libraries**: pandas, numpy, statsmodels, matplotlib, seaborn
- **Environment Management**: Resolving dependency and installation issues in conda/pip to ensure project stability
- **Code Quality**: Black formatter for PEP 8 compliance, clean notebook outputs
- **Business Impact**: Translating statistical findings into actionable recommendations

## Methodology
1. **Data Collection**: Q1 2025 student records from Calbright College
2. **Data Validation**: Manual verification of tutoring records against gradebook
3. **Statistical Modeling**: ZINB regression to handle overdispersed count data with excess zeros
4. **Validation**: Bootstrap analysis and permutation testing

## Strategic Student Segments Identified
- **Successful Engagement**: 67% of tutored students who made progress
- **Opportunity Group**: 33% of tutored students still at zero (targeted intervention needed)
- **Self-Starters**: 23% of untutored students who made progress independently
- **Challenge Group**: 77% of untutored students with no progress

## Results Summary
This analysis provided evidence-based recommendations that:
- Justified expansion of the tutoring program
- Identified specific student segments for targeted intervention
- Established a framework for ongoing program evaluation

## Data Privacy Note
All data files containing student information have been excluded from this repository to protect privacy. The notebooks demonstrate the analysis process and results without exposing sensitive information. 

To reproduce this analysis, you would need:
- Post tutor form data with student identifiers
- Gradebook export data from a learning management system
- Proper data access permissions

## Contact
[Masae Kobayashi Wen] - [mkwen2024@gmail.com] - [[LinkedIn](https://www.linkedin.com/in/masae-kobayashi-wen-42241a13/)]