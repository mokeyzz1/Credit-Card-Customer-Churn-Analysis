# Credit Card Churn & Retention Strategy

A comprehensive machine learning project that predicts customer churn and develops data-driven retention strategies for credit card companies. This analysis demonstrates how to build profitable churn prevention campaigns using business-optimized model thresholds.

## 🎯 Business Problem

Credit card companies lose substantial revenue when customers churn. Acquiring new customers costs 5-10x more than retaining existing ones, making churn prevention critical for profitability. This project develops a predictive model to identify at-risk customers and quantifies the ROI of targeted retention campaigns.

## 📊 Key Results

- **Net ROI**: $834,766 annually from churn prevention campaigns
- **ROI Multiple**: 10.52x return on investment
- **Model Performance**: 0.722 ROC AUC with profit-optimized threshold
- **Coverage**: 99.5% recall captures nearly all actual churners
- **Cost Efficiency**: Profitable even if intervention costs increase 10x

## 🚀 Project Overview

### Data Analysis
- **Dataset**: 10,000 credit card customers with 23 features
- **Target**: 11.1% churn rate (realistic for credit card industry)
- **Features**: Demographics, financial behavior, transaction patterns, risk metrics

### Model Development
- **Algorithms**: Logistic Regression, Gradient Boosting
- **Best Model**: Gradient Boosting with custom threshold optimization
- **Innovation**: Profit-maximizing threshold selection instead of accuracy-based

### Business Impact
- **Customers Saved**: 132 annually (after 60% campaign success rate)
- **Revenue Protected**: $889,416
- **Campaign Cost**: $87,650
- **Break-even Resilience**: Profitable even at 5.7% minimum success rate

## 📂 Project Structure

```
Credit Card Churn & Retention Strategy/
├── data/
│   ├── credit_card_customers.csv         # Raw dataset
│   └── credit_card_customers_cleaned.csv # Processed data
├── notebooks/
│   └── credit_card_churn_analysis.ipynb  # Main analysis notebook
└── README.md                             # This file
```

## 🔍 Analysis Stages

### Stage 1: Data Discovery & Understanding
- Exploratory data analysis of customer characteristics
- Data quality assessment and consistency checks
- Target variable analysis (11.1% churn rate)

### Stage 2: Data Quality & Cleaning
- Fixed tenure/relationship duration inconsistencies
- Handled missing values (income, payments, rewards)
- Standardized categorical variables
- Addressed negative values and data anomalies

### Stage 3: Exploratory Data Analysis
- **Key Finding**: Tenure is strongest churn predictor (-0.18 correlation)
- Customer segmentation by demographics and financial behavior
- Identified high-risk patterns: new customers, high utilization, low spending

### Stage 4: Feature Engineering
- Created business-meaningful features:
  - **CLV Proxy**: Monthly spend × tenure (customer lifetime value indicator)
  - **Engagement Score**: Transaction activity measure
  - **Risk-Adjusted Score**: Risk normalized by credit limit
  - **Utilization Categories**: Low/Medium/High credit usage

### Stage 5: Model Development & ROI Optimization
- Baseline models: Logistic Regression vs Gradient Boosting
- **Innovation**: Profit-optimized threshold selection
- Comprehensive ROI analysis with sensitivity testing
- Break-even analysis for different business scenarios

### Stage 6: Strategic Recommendations
- Deployment strategy with profit-tuned threshold (0.016)
- Customer segmentation for targeted campaigns
- Monitoring and recalibration framework
- Operational integration roadmap

## 💡 Key Insights

### Technical Insights
1. **Threshold Optimization**: Business-driven threshold selection dramatically improves ROI vs accuracy-based methods
2. **Precision vs Profit**: Low precision (12.5%) is acceptable when intervention costs are low relative to customer value
3. **Feature Importance**: Tenure, CLV proxy, and credit utilization are top churn predictors

### Business Insights
1. **High-Coverage Strategy**: Targeting broadly with cheap interventions beats precision targeting
2. **Financial Resilience**: Strategy remains profitable under wide range of cost/success scenarios
3. **Early Warning**: First 6-12 months are critical for customer retention

## 🛠️ Technical Stack

- **Python**: pandas, numpy, scikit-learn
- **Visualization**: matplotlib, seaborn
- **Machine Learning**: Logistic Regression, Gradient Boosting
- **Business Analytics**: ROI optimization, sensitivity analysis

## 📈 ROI Analysis Highlights

| Metric | Value |
|--------|--------|
| Annual Net ROI | $834,766 |
| ROI Multiple | 10.52x |
| Customers Saved | 132 |
| Campaign Cost | $87,650 |
| Break-even Cost | $526 per customer |
| Break-even Success Rate | 5.7% |

## 🎯 Strategic Recommendations

1. **Deploy Gradient Boosting Model** with profit-optimized threshold (0.016)
2. **Focus on Success Rate Improvement** from 60% to 75%+ for maximum ROI
3. **Implement Customer Segmentation** to prioritize high-value targets
4. **Monitor and Recalibrate** thresholds based on campaign results
5. **Test Precision-Boosting** strategies to reduce false positives

## 🚦 Getting Started

1. **Clone the repository**
2. **Install dependencies**: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`
3. **Run the notebook**: `notebooks/credit_card_churn_analysis.ipynb`
4. **Execute cells sequentially** for proper variable initialization

## 📋 Business Context

This analysis demonstrates enterprise-grade ML application with:
- **Profit-first methodology** over academic metrics
- **Realistic business assumptions** and sensitivity testing
- **Deployment-ready insights** with operational guidance
- **Stakeholder-friendly reporting** with clear ROI justification

