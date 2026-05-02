# stroke-prediction-ml
Machine Learning project to predict stroke using Logistic Regression, KNN, and Random Forest

#  Stroke Prediction Using Machine Learning

##  Project Overview
This project focuses on building and evaluating machine learning models to predict the likelihood of a stroke based on patient health data. Stroke prediction is a critical healthcare problem, where early detection can significantly improve patient outcomes and reduce risks.

---

##  Dataset Description
The dataset includes a variety of medical and demographic features such as:
- Age
- Gender
- Hypertension
- Heart disease
- Average glucose level
- Body Mass Index (BMI)
- Smoking status

The target variable is binary:
- **0** → No stroke  
- **1** → Stroke

---

##  Data Insights
- The dataset is **highly imbalanced**, with significantly fewer stroke cases.
- Missing values (e.g., BMI) were handled using appropriate imputation techniques.
- Certain features such as **age** and **glucose level** showed strong influence on predictions.

---

##  Models Implemented
We implemented and compared multiple machine learning models:

- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Random Forest  

Each model was evaluated in both its default form and after hyperparameter tuning using **GridSearchCV**.

---

##  Evaluation Strategy
Given the medical nature of the problem, we focused on:

- Confusion Matrix  
- Precision, Recall, and F1-score  
- **Recall (macro)** as the primary optimization metric  

This is because minimizing false negatives (missing actual stroke cases) is more critical than overall accuracy.

---

##  Best Model
The **Random Forest (tuned model)** achieved the best performance.

### Key Advantages:
- Improved recall for the stroke class (Class 1)
- Better balance between sensitivity and generalization
- Robust handling of feature interactions

---

##  Key Takeaway
In healthcare applications, **Recall is more important than Accuracy**.  
A model that correctly identifies more stroke cases is preferred, even if it introduces some false positives.

---

##  Conclusion
This project demonstrates how machine learning can be applied to real-world medical problems. By comparing multiple models and optimizing them, we were able to significantly improve predictive performance and build a more reliable stroke detection system.

---

##  Repository Contents
- `LogReg_Random_Forest_or_KNN.ipynb` → Full implementation and experiments
- README → Project summary and insights

---

##  Future Improvements
- Handle class imbalance using techniques like SMOTE
- Try advanced models (XGBoost, LightGBM)
- Deploy the model using a web interface (e.g., Streamlit)

---
