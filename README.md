# Pregnancy Risk Classification (Machine Learning)

## Author
**Elif Semiha Konakoğlu**


## Tech Stack
- Python
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn


## Notes
This project is created for educational and portfolio purposes.  
It is not intended for medical diagnosis or clinical use.

---

This project predicts **pregnancy risk level** using a clinical dataset and several supervised machine learning classification models.  
It includes data preprocessing, feature scaling, model training, and performance evaluation.

---

## Objective
To classify pregnancy cases into risk categories using clinical measurements and compare different machine learning models based on their performance.

---

## Dataset
- Clinical dataset used for pregnancy risk prediction  
- Target column: `risiko_cat`

### Getting the Dataset (Google Colab)
To run the notebook in Google Colab:
1. Keep the dataset ZIP file on your computer
2. Upload the ZIP file to Colab using the upload cell
3. Run all cells (the notebook extracts the ZIP and loads the CSV automatically)

Features include:
- Age  
- Blood pressure values (systolic / diastolic)  
- Hemoglobin (hb)  
- Medical conditions (e.g., diabetes, hypertension)  
- Other clinical indicators  

---

## Machine Learning Models
The following models were trained and compared:

- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Support Vector Machine (SVM - RBF kernel)  
- Random Forest  
- Gradient Boosting  

---

## Evaluation Metrics
Model performance was evaluated using:
- Accuracy  
- Precision (Macro)  
- Recall (Macro)  
- F1-score (Macro)  
- Confusion Matrix  
- Classification Report  

---

## Results (Summary)
| Model | Accuracy | Macro F1 |
|------|----------|----------|
| Logistic Regression | ~0.52 | ~0.42 |
| KNN | ~0.79 | ~0.61 |
| SVM (RBF) | ~0.76 | ~0.57 |
| Random Forest | ~0.90 | ~0.71 |
| **Gradient Boosting (Best)** | **~0.91** | **~0.74** |

**Best model:** Gradient Boosting

---

## Workflow
1. Upload & extract dataset (ZIP)
2. Load data with Pandas
3. Preprocess dataset
4. Train/test split
5. Standardize features using `StandardScaler`
6. Train multiple classification models
7. Compare models using evaluation metrics

---

## How to Run

### Google Colab (Recommended)
1. Open the notebook in Google Colab  
2. Upload the dataset ZIP file  
3. Run all cells  

### Run Locally (Optional)
1. Clone the repository  
2. Install dependencies  
3. Run the notebook  

```bash
pip install -r requirements.txt
jupyter notebook
