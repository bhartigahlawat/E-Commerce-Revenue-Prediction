# 🛒 E-Commerce Revenue Prediction using Machine Learning

## 📌 Overview
This project predicts whether a visitor on an e-commerce website will generate revenue (make a purchase) based on their browsing behavior and demographic information.  
The project uses a **Decision Tree Classifier** and demonstrates handling of categorical variables, overfitting control, and hyperparameter tuning.

---

## 🧠 Problem Statement
E-commerce businesses want to understand which visitors are likely to convert into paying customers.  
Predicting customer behavior can help target promotions, improve website design, and optimize marketing strategies.

---

## 📊 Dataset
- **Dataset Name:** Online Shoppers Purchasing Intention Dataset  
- **Source:** [Kaggle](https://www.kaggle.com/datasets)  
- **Features:** 17 features including session duration, page views, bounce rates, visitor type, and month  
- **Target Variable:** `Revenue`  
  - `0` → Visitor did not purchase  
  - `1` → Visitor made a purchase  

### Categorical Features
- `Month` → Month of visit  
- `VisitorType` → New or returning visitor  

Categorical features were handled using **one-hot encoding**.

---

## 🛠️ Tech Stack
- **Programming Language:** Python  
- **Libraries:**  
  - Pandas, NumPy → Data handling  
  - Matplotlib → Visualization  
  - Scikit-learn → Machine learning models  

---

## 🚀 Model Implementation
- **Model Used:** Decision Tree Classifier  
- **Train-Test Split:** 80-20%  
- **Hyperparameter Tuning:**  
  - `max_depth` → Controlled overfitting  
  - `min_samples_split` → Optimized tree performance  

### Accuracy
- Training Accuracy: ~0.92  
- Testing Accuracy: ~0.87  

> Hyperparameters were chosen to maximize test accuracy while preventing overfitting.

---

## 📈 Model Evaluation
- Overfitting detected by observing training vs testing accuracy  
- Optimized model parameters improved generalization  
- Confusion matrix and classification report can be generated for detailed performance metrics

---

## 📂 Project Structure
E-Commerce-Revenue-Prediction/
│── data/
│ └── shop_smart_ecommerce.csv
│── model.pkl
│── ecommerce_prediction.ipynb
│── README.md
│── requirements.txt

---

## ▶️ How to Run
1. Clone the repository:
```bash
git clone https://github.com/bhartigahlawat/E-Commerce-Revenue-Prediction.git

2. Navigate to the project folder:

cd E-Commerce-Revenue-Prediction


3. Install dependencies:

pip install -r requirements.txt


4. Run the notebook:

jupyter notebook
