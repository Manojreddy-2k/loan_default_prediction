# loan_default_prediction
## Abstract
This project aims to develop a machine learning-
based classification system to predict the likelihood of loan defaults
using the HMEQ dataset. Accurate prediction of loan defaults is
crucial for financial institutions to reduce credit risk and make
informed lending decisions. Multiple models—including Logistic
Regression, Decision Tree, Random Forest, XGBoost, and
LightGBM—were implemented and evaluated based on key
performance metrics such as Accuracy, Precision, Recall, F1-Score,
ROC AUC, and Brier Score. To balance predictive performance and
interpretability, SHAP (SHapley Additive exPlanations) was used to
explain model outputs, identifying features like DEBTINC, CLAGE,
and VALUE as influential. The XGBoost model emerged as the best-
performing model, offering high recall and model transparency via
SHAP. Threshold tuning was conducted to optimize decision-making
trade-offs between false positives and false negatives. This
interpretable framework provides a reliable and explainable
foundation for real-world loan risk assessment and deployment in
financial applications.
## INTRODUCTION AND MOTIVATION
### A. Background on Loan Defaults
Loan default occurs when a borrower fails to repay a loan
according to the agreed terms, resulting in financial loss for
lending institutions. With the rise in consumer borrowing,
especially in unsecured loans and home equity credit, the ability
to assess borrower risk has become increasingly critical.
Traditional credit scoring systems, while effective to some
extent, often fail to capture complex patterns in borrower
behavior, leading to misclassification of credit risk.
### B. Problem Statement
Financial institutions face the dual challenge of minimizing
default rates while ensuring fair and efficient lending practices.
Misjudging a customer’s likelihood of default can lead to either
financial losses or missed lending opportunities. This project
focuses on predicting loan defaults using machine learning
models applied to the HMEQ dataset, which contains borrower
financial and demographic attributes. The primary objective is
to build a model that accurately identifies potential defaulters
while maintaining transparency in decision-making.
### C. Importance of Interpretable Models
While advanced machine learning models like XGBoost and
LightGBM offer high predictive performance, their black-box
nature poses challenges in regulated domains like finance.
Model interpretability is essential for gaining trust from
decision-makers, complying with regulations, and
understanding feature influence. Using SHAP (SHapley
Additive exPlanations), this project aims to provide meaningful
explanations for model predictions, ensuring that the system is
both accurate and transparent.
### D. Goal of This Study
This study aims to develop and evaluate multiple
classification models—including Logistic Regression, Decision
Tree, Random Forest, XGBoost, and LightGBM—to predict the
likelihood of loan default. In addition to maximizing
performance metrics, the project emphasizes interpretability to
ensure the model’s outputs can be trusted by financial analysts
and credit officers. The ultimate goal is to provide a robust,
explainable machine learning framework that supports smarter,
data-driven lending decisions.
## OBJECTIVE
Our primary goal is to build an effective machine learning
pipeline to predict loan default while minimizing false
negatives. False negatives are critical in this context, as they
represent borrowers incorrectly classified as low risk,
potentially leading to financial loss for lending institutions.
To address this, we:
- Use multiple supervised learning algorithms, focusing on
interpretability and performance.
- Apply threshold optimization to tradeoff between precision
and recall.
- Evaluate each model using metrics like ROC-AUC and
Precision-Recall curves.
- Perform detailed analysis of misclassified examples.
