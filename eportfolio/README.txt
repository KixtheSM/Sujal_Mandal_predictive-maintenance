# CET313 - Artificial Intelligence Project  
**Predictive Maintenance for Industrial Equipment**  

## 📌 Project Overview  
A machine learning system to predict equipment failures using sensor data, achieving **98% accuracy** with Random Forest.  

---

## 📂 Weekly Progress  

### Week 1: Project Proposal  
- Selected NASA Turbofan Engine Degradation Dataset  
- Defined project scope and objectives  
- [Notebook](Week1_ProjectProposal.ipynb)  

### Week 2: Data Exploration  
- Analyzed distributions of sensor readings  
- Identified key correlations:  
  - `power` (rpm × torque) → -0.45 with failure  
  - `temp_diff` → 0.02 with failure  
- [Notebook](Week2_DataExploration.ipynb)  

### Week 3: Data Preprocessing  
- One-hot encoded categorical features (`Type`, `Failure Type`)  
- Scaled numerical features using `StandardScaler`  
- Train-test split (80/20)  
- [Notebook](Week3_DataPreprocessing.ipynb)  

### Week 4: Feature Engineering  
- Created new features:  
  - `power` = Rotational speed × Torque  
  - `temp_diff` = Process temp - Air temp  
  - Time-based wear rate  
- [Notebook](Week4_FeatureEngineering.ipynb)  

### Week 5: Model Training  
- Compared 3 models:  
  - Random Forest (98% accuracy)  
  - XGBoost (98.2%)  
  - Neural Network (97.5%)  
- Selected Random Forest after hyperparameter tuning  
- [Notebook](Week5_ModelTraining.ipynb)  

### Week 6: Model Evaluation  
- Key metrics:  
  - AUC-ROC: 0.99  
  - Recall (Failure class): 85%  
- [Notebook](Week6_ModelEvaluation.ipynb)  
![Confusion Matrix](confusion_matrix.png)  

### Week 7: Report Drafting  
- Generated technical report with:  
  - Methodology  
  - Results visualization  
  - Deployment recommendations  
- [Report Draft](draft_report.md)  

### Week 8: Finalization  
- Validated final model on fresh data  
- Compiled submission package:  
  - All notebooks  
  - Trained models (`*.pkl`)  
  - Final report  
- [Submission Checklist](checklist.md)  

---

## 🛠️ Technical Stack  
- Python 3.9  
- Libraries:  
  - `scikit-learn`, `XGBoost`, `pandas`, `matplotlib`  
- Dataset: [NASA Turbofan Degradation Data](https://ti.arc.nasa.gov/tech/dash/groups/pcoe/prognostic-data-repository/)  

---

## 📄 Final Deliverables  
1. [Final Report](final_report.md)  
2. [Trained Model](best_rf_model.pkl)  
3. [Complete Code](Week1-Week8_Notebooks.zip)  

---

## ✍️ Author  
Sujal Mandal
[University of Sunderland]  