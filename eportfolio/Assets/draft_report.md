
# CET313 Predictive Maintenance Report  
**Project:** Machine Failure Prediction  

## Key Results  
| Metric | Value |  
|--------|-------|  
| Accuracy | 0.98 |  
| Precision (Failure Class) | 0.92 |  
| Recall (Failure Class) | 0.85 |  
| AUC-ROC Score | 0.99 |  

## Insights  
1. The model achieves **98% accuracy** but has **15% false negatives** (missed failures).  
2. Top predictive features:  
   - `power` (engineered feature)  
   - `Torque [Nm]`  
   - `temp_diff`  

![Confusion Matrix](confusion_matrix.png)  
![ROC Curve](roc_curve.png)  

## Recommendations  
- Investigate false negatives with domain experts.  
- Deploy model with **85% recall threshold** for critical failures.  
