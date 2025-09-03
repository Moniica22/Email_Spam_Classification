# Email Spam Classification

This project develops and compares ML models to classify emails as **spam** or **ham**(not spam).  
**ML workflow**: dataset loading, preprocessing, feature extraction with TF-IDF, model training, hyperparameter tuning, and evaluation.

The dataset used is `spam_ham_dataset.xls`, with each row containing an email text and its corresponding label.

## Exploratory Data Analysis (EDA)
- Class balance analysis: spam vs ham distribution.
- Text cleaning with tokenization, stopword removal, and stemming.

## Feature Engineering
- **TF-IDF Vectorization** converts cleaned text into numerical vectors that represent word importance.  

##  Models Trained
Models tested and compared:
- **Logistic Regression**
- **Multinomial Naive Bayes**
- **Random Forest**
- **Linear Support Vector Classifier (LinearSVC)**

## Hyperparameter Tuning
We applied **GridSearchCV** with cross-validation to the best-performing model(**LinearSVC**, with accuracy: 0.99).  
- **Best parameters found:**  
  `C = 1`, `loss = squared_hinge`, `max_iter = 1000`  
- **Best CV F1:** ≈ 0.982

## Ejecution
1. Clone the repository:
```
git clone https://github.com/Moniica22/Email_Spam_Classification.git
cd Email_Spam_Classification
```
2. Install dependencies
```
pip install -r Requirements.txt
```
3. Run Jupyter notebook
```
jupyter notebook Email_Spam_Classif.ipynb
```



## License
MIT (or your preferred license).
