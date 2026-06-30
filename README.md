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
1. **Logistic Regression** (Best Model) ⭐
   - ROC-AUC: 0.7986 (79.86%)
   - F1-Score: 0.4394
   - Most interpretable for HR teams
   
2. **Random Forest Classifier**
   - Ensemble method with 100 trees
   - Handles non-linear relationships
   
3. **Gradient Boosting Classifier**
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
EmployeeAttrition/
├── analysis.ipynb # Complete notebook (all 7 tasks)
├── WA_Fn-UseC_-HR-Employee-Attrition.csv # Dataset (1,470 employees)
├── summary.pdf # Executive summary (non-technical)
├── README.md # This file
└── charts/ # Visualizations
├── chart1_attrition_by_department.png
├── chart2_income_comparison.png
├── chart3_confusion_matrix.png
├── chart4_feature_importance.png
└── chart5_roc_curves.png


## 📋 Tasks Completed

✅ **Task 1:** Data Loading & Exploration (1,470 employees, 35 features)  
✅ **Task 2:** Data Cleaning & Preprocessing (handled imbalance, encoding, scaling)  
✅ **Task 3:** EDA (department, role, income, work-life balance analysis)  
✅ **Task 4:** Model Building (3 models trained, 80/20 split)  
✅ **Task 5:** Model Evaluation (precision, recall, F1, ROC-AUC, confusion matrix)  
✅ **Task 6:** Visualizations (5 professional charts)  
✅ **Task 7:** HR Insights & Recommendations (non-technical summary)

## 🛠️ Technologies Used

**Core Stack:**
- Python 3.x
- Jupyter Notebook / Google Colab

**Libraries:**
- Pandas (data manipulation)
- NumPy (numerical operations)
- Scikit-learn (ML models & preprocessing)
- Matplotlib & Seaborn (visualizations)

**ML Techniques:**
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