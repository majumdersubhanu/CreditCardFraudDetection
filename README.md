# Credit Card Fraud Detection: A GCRISP-DS-Based Approach

This repository presents an end-to-end implementation of a fraud detection system using the **GCRISP-DS framework**. The
goal is to identify fraudulent credit card transactions using machine learning models while ensuring reproducibility,
academic rigor, and practical deployment potential.

## 📌 Framework Used

This project follows the **GCRISP-DS** data science methodology:

- Goal: Define the problem in business and technical terms
- Context: Understand the domain, stakeholders, and constraints
- Requirements: Define data, metrics, and tools
- Insights: Perform deep exploratory analysis
- Solutions: Build and evaluate multiple machine learning models
- Productization: Prepare model for real-world deployment

---

## 📁 Repository Structure

```text
├── data/ # Contains saved model artifacts (not tracked in Git)
├── fraud_detection_report.ipynb # Main notebook with GCRISP-DS-based analysis
├── README.md
````

> 📌 **Note**: The dataset and trained models are **not included** in this repository due to size and privacy
> restrictions.

---

## 📊 Dataset

The dataset used in this project is available from Kaggle:

🔗 [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

- **Size**: ~150 MB
- **Records**: 284,807 transactions
- **Features**: 30 anonymized + 1 target variable (`Class`)
- **Class Imbalance**: Only ~0.17% of transactions are fraudulent

---

## ⚙️ Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/majumdersubhanu/CreditCardFraudDetection.git ml_project
   cd ml_project
   ```

2. **Create and activate a virtual environment (optional but recommended):**

   ```bash
   python -m venv venv
   source venv/bin/activate    # On Windows use: venv\Scripts\activate
   ```

3. **Install required dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Download the dataset from Kaggle:**

    * Visit the [dataset page](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
    * Download and unzip it into a folder named `data/`
    * The file should be placed at `data/creditcard.csv`

5. **Run the main notebook:**
    * Open and execute the following notebooks in order:
        * `data_exploration.ipynb`.
        * `data_preprocessing.ipynb`.
        * `fraud_detection_report.ipynb`.

---

## ✅ Features

* Exploratory Data Analysis (EDA) with visual insights
* Preprocessing: Standardization, SMOTE for class balancing
* Models used:

    * Logistic Regression
    * Random Forest
    * XGBoost
* Visual comparisons:

    * Confusion matrices
    * ROC curves
* Model persistence with `.json` export
* Scalable code structure with academic documentation

---

## 📦 Dependencies

Minimal `requirements.txt`:

```
pandas
numpy
scikit-learn
imblearn
xgboost
matplotlib
seaborn
```

---

## ✍️ Author

Made with 💗 by Subhanu Majumder

[LinkedIn](https://linkedin.com/in/subhanumajumder) | [GitHub](https://github.com/majumdersubhanu/)

---

## 📜 License

This project is released under the MIT License. You are free to use, modify, and distribute it with attribution.
