# Student-Dropout-Classifier

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=flat&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Status](https://img.shields.io/badge/Project-Completed-success)

##  Project Overview
**Can we predict student dropout before it happens?**
This project leverages Machine Learning to build an **Early Warning System** for educational institutions. By analyzing demographic, socioeconomic, and academic data, the model identifies students at risk of failure, enabling proactive intervention to improve retention rates.

##  Key Technical Skills
This project demonstrates an end-to-end Data Science workflow:
*   **SQL Integration:** Simulated an enterprise environment by converting raw CSV data into a **SQLite database** and querying it using Python.
*   **Handling Imbalanced Data:** Applied **SMOTE** (Synthetic Minority Over-sampling Technique) to address the scarcity of dropout cases, ensuring the model is not biased towards the majority class.
*   **Robust Preprocessing:** Implemented **Stratified Splitting** to maintain class distribution integrity during training/testing.
*   **Predictive Modeling:** Built and optimized a **Random Forest Classifier**.
*   **Business Interpretability:** Extracted **Feature Importance** to explain the root causes of dropout.

##  Model Performance
The model achieved strong performance metrics on the test set, proving its reliability for real-world application:

| Metric | Score | Interpretation |
| :--- | :--- | :--- |
| **ROC-AUC** | **0.93** | Excellent capability in distinguishing between at-risk and safe students. |
| **Accuracy** | **88%** | High overall correctness. |
| **Recall (Dropout)**| **78%** | Successfully captures 78% of actual dropouts (Crucial for minimizing False Negatives). |

###  Confusion Matrix & ROI
The model successfully flagged a significant number of at-risk students who would have otherwise been missed. In an educational context, this translates to:
- **Early Intervention:** Advisors can focus on students flagged by the model.
- **Resource Optimization:** Targeting support where it's needed most.

## 🔍 Key Insights (Drivers of Dropout)
Based on the Feature Importance analysis, the top factors predicting dropout are:
1.  **2nd Semester Academic Performance:** Grades and approved units in the 2nd semester are the strongest predictors.
2.  **Tuition Fees Status:** Financial distress (failure to pay fees) is a critical early warning sign.
3.  **Age at Enrollment:** Older students tend to face higher risks of dropping out.

## 🚀 How to Run
1.  **Clone the repository:**
  
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the Notebook:**
    Open `Student_Dropout_Classifier.ipynb` in Jupyter Notebook or Google Colab.
    *(Ensure `dataset.csv` is in the same directory)*.

## 📂 Project Structure
```text
├── data                    # Dataset file (csv)
├── notebook                # Jupyter Notebook with full analysis & code
├── README.md               # Project documentation
└── requirements.txt        # Dependencies
