# HR Employee Turnover Prediction

![Python](https://img.shields.io/badge/Python-3.8+-blue) ![Machine Learning](https://img.shields.io/badge/ML-Classification-orange) ![Industry](https://img.shields.io/badge/Industry-HR_Analytics-green)

**Machine learning application for predicting employee turnover using HR data**

*Google Advanced Data Analytics Capstone Project - Employee retention analysis and predictive modeling*

## Project Overview

Machine learning application for predicting employee turnover at Salifort Motors using employee performance and satisfaction data. This project demonstrates end-to-end data science capabilities in human resources analytics, focusing on identifying key factors driving employee departures and building predictive models for proactive retention strategies.

**Result: 99.09% accuracy in employee turnover prediction using Random Forest**

## Business Problem

Salifort Motors faces a critical employee retention challenge with 24.5% annual turnover rate, significantly higher than industry standards. High turnover results in substantial recruitment costs, disrupted project continuity, and loss of institutional knowledge. This project develops a predictive framework to identify at-risk employees before they leave, enabling targeted retention interventions.

### Dataset Characteristics
- 13,717 employee records across 10 departments
- Class distribution: 75.5% Stayed vs 24.5% Left (manageable imbalance)
- Features: satisfaction level, performance evaluation, project count, work hours, tenure, promotions, salary, department
- No missing values, minimal data cleaning required

## Technical Approach

### Data Pipeline
1. **Data Exploration**: Comprehensive EDA with correlation analysis and statistical testing
2. **Data Cleaning**: Outlier detection and removal for tenure variable
3. **Feature Engineering**: One-hot encoding for categorical variables, appropriate scaling
4. **Model Development**: Systematic comparison of classification algorithms

### Model Performance Comparison

| Model | Accuracy | Precision | Recall | F1-Score | ROC AUC | Approach |
|-------|----------|-----------|--------|----------|---------|----------|
| Logistic Regression | 81.6% | 64.3% | 55.9% | 59.8% | 87.9% | Baseline linear model |
| **Random Forest** | **99.1%** | **99.4%** | **96.9%** | **98.1%** | **99.1%** | **Balanced ensemble method** |

## Key Technical Components

### Statistical Analysis Framework
- **Point-biserial correlation**: Continuous-binary variable relationships
- **Cramér's V**: Categorical association testing
- **Significance testing**: Hypothesis validation for key relationships

### Feature Importance Analysis
**SHAP Implementation:**
1. **Satisfaction Level**: 30.9% importance - strongest predictor
2. **Tenure**: 24.9% importance - longer tenure correlates with higher turnover
3. **Project Count**: 16.7% importance - overload indicator (6+ projects = 85% departure probability)
4. **Work Hours**: 12.2% importance - work-life balance metric (250+ hours critical threshold)
5. **Performance Evaluation**: 11.0% importance - high performers leaving at higher rates

### Key Findings

**Critical Risk Factors:**
- **Satisfaction Level**: -0.39 correlation with turnover (highly significant)
- **Tenure Pattern**: Experienced employees (4+ years) showing highest departure rates
- **Project Load**: Clear burnout indicator at 6+ simultaneous projects
- **Performance Factor**: High-performing employees leaving more frequently

**Departmental Analysis:**
- Sales & Technical departments: Highest turnover rates
- Low-salary employees: 3x more likely to leave
- Management with medium salaries: Notable 34% turnover rate

### Model Interpretability
- **Global Feature Importance**: Clear ranking of turnover drivers
- **SHAP Analysis**: Individual prediction explanations for targeted interventions
- **Statistical Validation**: All key relationships confirmed with significance testing
- **Business Alignment**: Feature importance matches domain expertise expectations

## Results & Business Impact

### Model Performance
- **99.09% Accuracy**: Strong overall classification performance
- **96.88% Recall**: Successfully identifies 97% of employees likely to leave
- **3.1% False Negative Rate**: Low rate of missed departures for retention opportunities

### Operational Recommendations
1. **Immediate Actions**: Deploy quarterly at-risk employee identification
2. **Workload Management**: Cap projects at 4-5 per employee, maximum 200 hours/month
3. **Satisfaction Monitoring**: Implement pulse surveys for real-time tracking
4. **Retention Programs**: Target high-performers and experienced staff

### Business Value
- **Proactive Retention**: Identify 97% of at-risk employees before departure
- **Cost Reduction**: Potential 60-80% reduction in turnover-related costs
- **Strategic Planning**: Data-driven HR policy improvements
- **Departmental Focus**: Targeted interventions for high-risk areas

## Technologies & Skills

**Analytics Stack:**
- **ML Framework**: Scikit-learn with Random Forest optimization
- **Statistical Analysis**: SciPy for correlation testing and hypothesis validation
- **Interpretability**: SHAP for feature importance and model explanation
- **Visualization**: Matplotlib, Seaborn for comprehensive EDA

**Business Skills:**
- **HR Analytics**: Employee lifecycle and retention factor analysis
- **Statistical Testing**: Appropriate test selection for different variable types
- **Stakeholder Communication**: Executive presentation and actionable recommendations
- **ROI Analysis**: Business impact quantification and cost-benefit assessment

## Project Structure

```
├── notebooks/              # Analysis and modeling code
├── visualizations/         # Tableau dashboards and analysis
├── docs/                   # PACE documentation and Executive Summary Slides
└── README.md               # Project overview
```

## Results Summary

### Technical Achievements
- **Target Performance**: 99.09% accuracy vs 85%+ target requirement
- **Model Selection**: Random Forest optimal without hyperparameter tuning
- **Feature Engineering**: Effective categorical encoding and outlier management
- **Statistical Rigor**: Comprehensive correlation analysis with significance testing

### Business Insights
- **Satisfaction Level**: Most critical factor requiring immediate attention
- **Project Load**: Clear operational threshold identified (6+ projects)
- **Tenure Pattern**: Experienced employees need retention focus
- **Department Strategy**: Sales & Technical require targeted interventions

### Implementation Ready
- **Quarterly Deployment**: Model ready for at-risk employee identification
- **Action Framework**: Clear retention protocols based on risk scores
- **Performance Monitoring**: Systematic tracking and model updating procedures
- **Cost-Benefit Analysis**: Quantified ROI for retention program investment

## Limitations & Future Work

### Current Scope
- **Single Company Data**: Model trained on Salifort Motors specific patterns
- **Historical Analysis**: No real-time integration or dynamic updating
- **Limited Features**: Standard HR metrics without external market factors

### Enhancement Roadmap
**Technical Improvements:**
- Real-time data pipeline integration
- External market factor incorporation (salary benchmarks, industry trends)
- Advanced ensemble methods for improved robustness
- Automated model retraining and performance monitoring

**Business Applications:**
- Cross-industry model validation and adaptation
- Manager effectiveness integration
- Early warning system automation
- Personalized retention recommendation engine

## Conclusion

This project demonstrates the application of machine learning to critical HR challenges, achieving strong predictive performance while maintaining clear business focus. The Random Forest model provides reliable employee turnover prediction with actionable insights for retention strategy development.

The work establishes a foundation for data-driven HR decision making, transforming reactive hiring practices into proactive talent retention through systematic risk identification and targeted intervention capabilities.

---

**About:** This project represents practical application of data science to human resources challenges, demonstrating technical proficiency in classification modeling while maintaining clear focus on business value creation and operational implementation.
