# Fraud-Detection
**_A machine learning model to detect the fraudulent transactions_**.

## Download the data ##
Download the dataset (_csv format_) from [here](https://www.kaggle.com/mlg-ulb/creditcardfraud/data).

## Installation ##
Anaconda is highly recommended for executing any data science projects. It comes with a lots of pre-installed packages for data analysis and machine learning. Two packages needs to be manually installed beside installing Anaconda.

* Seaborn (_pip install seaborn_ or _conda install seaborn_)
* Imbalanced-learn (_pip install -U imbalanced-learn_)

## Summary ##
This notebook can be devided into the following sections:
* **_Data exploration_**
* **_Feature engineering_**
* **_Evaluation metrics_**
* **_Modeling_**
* **_Parameter tuning_**

After initial exploration, the dataset turns out to be highly imbalanced. Normal machine learning algorithms are biased 
towards the majority class. Resampling technique has been used to handle this problem. New features are generated based on the distribution of variables with in class. The accuracy metric is not useful for imbalanced class, so f1 ( _harmonic mean of precision and recall_ ) and auc ( _area under the roc curve are used to evaluate the model performance_). The usual threshold (_probability = 0.5_) is not used for classification. It has been tuned using cross-validation strategy.





