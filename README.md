# Cancer-prediction-using-SVM
# 🧠 Breast Cancer Classification using SVM

This project uses a **Support Vector Machine (SVM)** to classify breast cancer tumors as **benign** or **malignant** based on diagnostic features. The model is trained and evaluated using the **Breast Cancer Wisconsin dataset**, a benchmark dataset widely used in machine learning and healthcare classification tasks.

---

## 🛠️ How I Built It

This project was built entirely inside a Jupyter Notebook using the following steps:

1. **📥 Data Loading**  
   - I used the `load_breast_cancer()` function from `sklearn.datasets` to load the Breast Cancer Wisconsin Diagnostic dataset.  
   - I converted the data into a `pandas.DataFrame` for easier manipulation and visualization.

2. **📊 Data Understanding & Exploration**  
   - Checked dataset shape, feature names, target values, and class balance.  
   - Verified there were no null or missing values.  
   - Visualized class distributions to understand the benign vs malignant breakdown.

3. **🧹 Data Preprocessing**  
   - Split the dataset into features (`X`) and target (`y`).  
   - Used `StandardScaler` to normalize the features (since SVMs are sensitive to scale).  
   - Split the data into training and testing sets using `train_test_split`.

4. **🤖 Model Building**  
   - Used `sklearn.svm.SVC` to create an SVM model.  
   - Trained the model using the training data.  
   - I chose default hyperparameters, but these can be tuned later for optimization.

5. **📈 Model Evaluation**  
   - Evaluated the model using `accuracy_score`, `confusion_matrix`, and `classification_report`.  
   - Accuracy was around 96–98%, with high precision and recall.

6. **🧠 Making Predictions**  
   - I demonstrated prediction on new sample input (manually entered).  
   - The model classifies the result as either `Benign` or `Malignant` based on the trained SVM.

7. **🖼️ Visualization**  
   - Used `seaborn` and `matplotlib` to plot the confusion matrix and dataset insights.

---

## 📂 Project Structure

- `cancersvm.ipynb` – Main notebook with all steps from data loading to evaluation
- Dataset: Comes from `sklearn` (no need to download externally)

---

## 🚀 Workflow Overview

1. Data Loading  
2. Data Cleaning & Normalization  
3. SVM Model Training  
4. Evaluation (Confusion Matrix, Accuracy)  
5. Prediction Demo  
6. Visualization

---

## 📊 Sample Results

| Metric       | Value     |
|--------------|-----------|
| Accuracy     | ~97%      |
| Precision    | High      |
| Recall       | High      |
| Confusion Matrix | ✅ Clean separation between benign & malignant |

---

## 📦 Libraries Used

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

---

## 🧪 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/cancersvm.git
   cd cancersvm
