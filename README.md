# Age Group Prediction using NHANES Data
This repository contains my solution for the **Summer Analytics 2025 Hackathon** hosted by the **Consulting and Analytics Club, IIT Guwahati**, focused on predicting whether a person is a **Senior (65+)** or **Adult (<65)** using the NHANES dataset.

## 📌 Problem Statement
Participants are provided with health and nutritional data collected from the NHANES study. The objective is to build a binary classification model that predicts whether a respondent is a Senior (1) or an Adult (0) based on health and lifestyle features.

## 🧠 Task
- Predict the `age_group`:
  - `0` → Adult (< 65 years)
  - `1` → Senior (≥ 65 years)
- Evaluation metric: **F1 Score**

## 📁 Dataset Description
- `Train_Data.csv`: Contains 2,016 records with features and the target variable `age_group`.
- `Test_Data.csv`: Contains 312 records (target variable hidden).
- `Sample_Submission.csv`: Format for final submission.

### Features
| Feature | Description |
|---------|-------------|
| SEQN | Respondent ID |
| RIAGENDR | Gender (1=Male, 2=Female) |
| PAQ605 | Physical activity participation |
| BMXBMI | Body Mass Index |
| LBXGLU | Glucose level |
| DIQ010 | Diabetes questionnaire |
| LBXGLT | Oral glucose tolerance |
| LBXIN | Insulin level |

## 🔍 Approach
1. **EDA**: Identified distributions, missing values, and feature correlations.
2. **Data Cleaning**: Handled missing values using appropriate imputation.
3. **Feature Engineering**: Encoded categorical values and normalized continuous features.
4. **Modeling**: Trained various classification models (Random Forest, Logistic Regression, etc.)
5. **Evaluation**: Chose the best model based on F1 score using cross-validation.
6. **Prediction**: Predicted labels on test set and exported results to `Submission.csv`.

## 📦 Libraries Used
- `pandas`
- `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`

## 🧾 Output
The final output is a `Submission.csv` file containing the predicted `age_group` values for the test dataset.

```csv
age_group
0
1
0
...
📜 Instructions to Run
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/age-group-prediction.git
cd age-group-prediction
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the notebook:
Open AI_hackathon.ipynb in Jupyter Notebook or VSCode and run all cells.

Export the predictions:
The notebook generates Submission.csv automatically.

🏁 Final Notes
This solution is submitted for Summer Analytics 2025 hosted by CnA Club, IITG.

The model is optimized for F1 score.

All files in this repo are for educational and non-commercial use only.

© 2025 | Created by [Your Name]

yaml
Copy
Edit

---

### Optional Add-ons:
- Rename your notebook to `AI_hackathon.ipynb` or `NHANES_Age_Prediction.ipynb` for clarity.
- Add a `requirements.txt` file (I can generate it for you if needed).

Let me know if you want me to generate that file or customize the README with your name or GitHub 
