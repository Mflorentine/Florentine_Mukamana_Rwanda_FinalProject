## Early Sepsis Risk Prediction in Intensive Care Unit Using Machine Learning

This project explores machine learning approaches for early sepsis risk prediction using ICU data. The goal is to evaluate models as early‑warning decision support tools, not automated diagnostic systems, 
with emphasis on clinically meaningful evaluation, recall, and calibrated risk estimation.
## Dataset
- **Original source:** PhysioNet / Computing in Cardiology (CinC) 2019 Sepsis Challenge  
  https://physionet.org/content/challenge-2019/1.0.0/  
- Also accessed via Kaggle:  
  https://www.kaggle.com/datasets/tea340yashjoshi/sepsis-prediction-dataset  
The dataset contains hourly ICU measurements for individual patients with a binary label indicating sepsis risk within six hours before clinical recognition.
## Methods
The study uses Logistic Regression, Random Forest, and Gradient Boosting models to compare linear and tree‑based approaches for early sepsis risk prediction.
Median imputation is applied to handle missing values in ICU measurements as a pragmatic baseline.
Model performance is evaluated using clinically meaningful metrics, with emphasis on ROC‑AUC, recall, classification reports, and confusion matrices, rather than accuracy.
A recall‑focused probability threshold (0.25) is applied to predicted probabilities to reduce missed sepsis cases.
Probability calibration (Platt scaling) is performed for Logistic Regression and Random Forest to improve the interpretability and reliability of predicted risk scores.
## Key Results
- Random Forest achieved the highest ROC‑AUC (≈ 0.79)  
- ROC‑AUC alone was insufficient in this imbalanced setting  
- Recall‑focused analysis and probability calibration were essential for meaningful early‑warning risk estimation
  
This project can be used for educational and methodological demonstration of sepsis risk prediction and evaluation strategies. Not for direct clinical deployment.
