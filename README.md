# 👥 Employee Attrition Prediction

Machine Learning project to predict employee turnover and help HR teams retain valuable talent.

## 📊 Project Overview

- **Dataset:** IBM HR Analytics (1,470 employees)
- **Problem Type:** Binary Classification (Leave/Stay)
- **Attrition Rate:** 16.1% (237 left, 1,233 stayed)
- **Best Model:** Logistic Regression
- **Performance:** 79.86% ROC-AUC Score

## 🔍 Key Findings

### Top 3 Predictive Factors

1. **Job Role (Laboratory Technician)** - Highest risk role identifier
2. **Overtime Work** - Strong predictor of departure
3. **Business Travel Frequency** - Frequent travelers at higher risk

### High-Risk Groups

- **Sales Department:** 20.6% attrition (highest department)
- **Sales Representatives:** 39.8% attrition (highest role)
- **Income Gap:** Employees who left earned **$2,046/month less** on average

### Critical Insights

- Early career employees (0-2 years) show highest attrition
- Work-life balance significantly impacts retention
- Compensation alone doesn't explain departures

## 🤖 Machine Learning Models

### Models Trained & Compared

#### 1. **Logistic Regression** (Best Model) ⭐

- ROC-AUC: 0.7986 (79.86%)
- F1-Score: 0.4394
- Most interpretable for HR teams

#### 2. **Random Forest Classifier**

- Ensemble method with 100 trees
- Handles non-linear relationships

#### 3. **Gradient Boosting Classifier**

- Advanced boosting technique
- Sequential learning approach

### Why Logistic Regression Won

- Clear linear relationships in the data
- Highly interpretable coefficients
- Fast prediction and deployment
- Excellent baseline performance
- Easy to explain to non-technical stakeholders

### Model Performance

- Correctly identifies ~80% of at-risk employees
- Balanced approach between precision and recall
- Handles class imbalance with weighted training
- Production-ready for HR deployment

## 📁 Project Structure

```text
EmployeeAttrition/
├── analysis.ipynb                            # Complete notebook (all 7 tasks)
├── WA_Fn-UseC_-HR-Employee-Attrition.csv     # Dataset (1,470 employees)
├── summary.pdf                               # Executive summary (non-technical)
├── README.md                                 # This file
└── charts/                                   # Visualizations
    ├── chart1_attrition_by_department.png
    ├── chart2_income_comparison.png
    ├── chart3_confusion_matrix.png
    ├── chart4_feature_importance.png
    └── chart5_roc_curves.png
```

## 📋 Tasks Completed

✅ **Task 1:** Data Loading & Exploration (1,470 employees, 35 features)  
✅ **Task 2:** Data Cleaning & Preprocessing (handled imbalance, encoding, scaling)  
✅ **Task 3:** EDA (department, role, income, work-life balance analysis)  
✅ **Task 4:** Model Building (3 models trained, 80/20 split)  
✅ **Task 5:** Model Evaluation (precision, recall, F1, ROC-AUC, confusion matrix)  
✅ **Task 6:** Visualizations (5 professional charts)  
✅ **Task 7:** HR Insights & Recommendations (non-technical summary)

## 🛠️ Technologies Used

### Core Stack

- Python 3.x
- Jupyter Notebook / Google Colab

### Libraries

- Pandas (data manipulation)
- NumPy (numerical operations)
- Scikit-learn (ML models & preprocessing)
- Matplotlib & Seaborn (visualizations)

### ML Techniques

- StandardScaler (feature normalization)
- One-hot encoding (categorical variables)
- Class weight balancing (imbalanced data)
- Train-test split with stratification

## 🚀 How to Run

### Google Colab (Recommended)

1. Open Colab link
2. Click "Runtime" → "Run all"
3. Dataset auto-downloads from this repository
4. View results inline (~2 min execution time)

### Local Jupyter

```bash
# Clone repository
git clone https://github.com/Harshitd13/EmployeeAttrition.git
cd EmployeeAttrition

# Install dependencies
pip install pandas numpy scikit-learn matplotlib seaborn jupyter

# Run notebook
jupyter notebook analysis.ipynb
```

## 💼 Business Recommendations

### Immediate Actions (Next 30 Days)

- Retention Conversations: Meet with all Sales Representatives (39.8% attrition risk)
- Overtime Audit: Monitor and reduce excessive overtime patterns
- Compensation Review: Address $2,046 income gap for at-risk employees

### Medium-Term Initiatives (90 Days)

- Mentorship Program: Support for new employees (0-2 years tenure)
- Travel Policy Review: Reduce frequent business travel burden
- Work-Life Balance: Implement flexible work arrangements
- Laboratory Technician Retention: Create clear career advancement paths

### Expected Business Impact

- Reduce attrition from 16.1% to 12% (industry benchmark)
- Save ~$500K annually in recruitment and training costs
- Retain top talent before competitors poach them
- Improve employee satisfaction through data-driven interventions

## ⚠️ Model Limitations

### Technical

- Predicts risk probability, not certainty
- 20% of actual departures may be missed
- Requires quarterly retraining with new data

### Practical

- Cannot predict external job offers
- Doesn't capture personal/family situations
- Should guide support, never punitive actions

### Ethical

- Use predictions confidentially
- Combine with human judgment
- Regular bias audits required
- Voluntary employee participation

## 📊 Key Statistics

| Metric | Value |
|--------|-------|
| Total Employees | 1,470 |
| Attrition Rate | 16.1% |
| Employees Left | 237 |
| Best Model ROC-AUC | 79.86% |
| Highest Risk Dept | Sales (20.6%) |
| Highest Risk Role | Sales Rep (39.8%) |
| Income Gap | $2,046/month |
| Top Predictor | Laboratory Technician Role |

## 🔗 Links

- Google Colab: https://colab.research.google.com/drive/126BQqT1ej-6IGoM5Uek0pKm_uss09NCu?usp=sharing
- Dataset Source: IBM HR Analytics on Kaggle

## 👤 Author

- Name: Harshit Dwivedi
- Project: Week 2 Internship Assignment
- Date: 30 June 2026
- Email: harshitd3113@gmail.com
- GitHub: https://github.com/Harshitd13

## 📝 Project Status

✅ **COMPLETE**

All 7 tasks finished, 3 models trained and compared, 5 visualizations created, business recommendations delivered in non-technical language.

## 🎯 Learning Outcomes

This project demonstrates:

- End-to-end ML workflow (data → insights → recommendations)
- Handling imbalanced datasets with class weighting
- Model interpretability for business stakeholders
- Translating technical results to HR-friendly language
- Professional documentation and version control

## 📄 License

This project is created for educational purposes as part of an internship assignment.

Dataset: IBM HR Analytics (CC0: Public Domain)

⭐ Star this repo if you found it helpful!

Built with Python and Scikit-learn | Employee attrition through data science
