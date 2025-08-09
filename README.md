# Credit Card Approval Prediction

This project implements a **machine learning pipeline** to predict whether a credit card application will be approved based on applicant details.  
The model is trained using the **Logistic Regression** algorithm, with preprocessing steps to handle missing values, encode categorical features, and scale numeric features.

## 📂 Dataset
The dataset used is **`cc_approvals.data`**, which contains applicant details such as age, income, credit history, and more.  
Some values are missing (represented as `?`), which are handled during preprocessing.

---

## 🔄 Workflow
1. **Data Loading & Exploration**  
   - Read dataset into Pandas DataFrame  
   - Generate summary statistics and check data types  

2. **Data Preprocessing**  
   - Replace missing values with mean (for numeric) or mode (for categorical)  
   - Encode categorical features using **Label Encoding**  
   - Drop irrelevant columns (11 and 13)  
   - Scale features using **MinMaxScaler**  

3. **Model Training**  
   - Train a **Logistic Regression** model  
   - Evaluate with accuracy score and confusion matrix  

4. **Hyperparameter Tuning**  
   - Use **GridSearchCV** to find best `tol` and `max_iter` values  

---

## 📊 Results
- The model achieves an accuracy of **84%**.

---

## 🛠 Tech Stack
- **Python**  
- **Pandas**, **NumPy**  
- **Scikit-learn**  

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/muditvir/cc_approvals.git
   cd cc_approvals
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn
   ```
3. Run the script:
   ```bash
   python credit_card_approval.py
   ```
