# SECOM_class_imbalance
Approaches for the class imbalance problem (in semicondutor manufacturing process line data)


### Description
The SECOM dataset in the UCI Machine Learning Repository is semicondutor manufacturing data which has 1567 records, 590 anonymized features and 104 fails. The process yield has a simple pass/fail response (encoded -1/1).

The dataset has the following characteristics:

1.	two-class problem
2.	an imbalance with a 14:1 skew of pass to fails
2.	large number of features -- 590
3.	missing data
4.	features/columns which do not have sufficient information
  5.	4% of the columns/features have more than 50% of their records missing
  6.	some columns have constant values 

### Objective
The SECOM dataset presents us with two problems: (i) working with skewed data and (ii) feature selection. 
The main focus for this analysis will be the class imbalance issue and the ability to successfully predict fails. Strategies used in fraud/anomaly detection/rare disease diagnosis will be useful here. 
A secondary objective will be feature reduction. (In some to the literature pertaining to the SECOM dataset, this was the primary goal <a href="#ref1">[1]</a>.) A streamlined feature set can not only lead to better prediction accuracy and data understanding but also save manufacturing resources. 

###Software

- Python 2.7
- scikit-learn packages for algorithms
- pandas for data wrangling 
- Matplotlib and Seaborn for plotting and visualization

###Methods
We will look at some of the approaches that deal with class imbalance. These can be a cost sensitive learning approach or sampling-based. We will also be working with feature selection methods. We will begin with the following:

1. [Random Forest variable importance (feature selection)](https://github.com/Meena-Mani/SECOM_class_imbalance/blob/master/secomdata_ocsvm.ipynb)
2. [One-class SVM](https://github.com/Meena-Mani/SECOM_class_imbalance/blob/master/secomdata_ocsvm.ipynb) 
3. [SVM with SMOTE (oversampling minority class/undersampling majority class)](https://github.com/Meena-Mani/SECOM_class_imbalance/blob/master/secomdata_svm_smote.ipynb)
4. [SVM, Undersampling and Data Cleaning for Imbalanced Data](https://github.com/Meena-Mani/SECOM_class_imbalance/blob/master/secomdata_svm_undersampling.ipynb)
5. [Random Forest (weighting the classes)](https://github.com/Meena-Mani/SECOM_class_imbalance/blob/master/secomdata_rf.ipynb)
6. Boosting methods

This is Work-In-Progress so new exercises will be added and old ones refined on an on-going basis.

###Further Reading
<a name="ref1"></a>[1] [McCann, Michael, et al. "Causality Challenge: Benchmarking relevant signal components for effective monitoring and process control." NIPS Causality: Objectives and Assessment.2010.](https://scholar.google.com/scholar?cluster=9582225450011234329&hl=en&as_sdt=0,5&sciodt=0,5)  
<a name="ref2"></a>[2] [H. He and E. A. Garcia, “Learning from Imbalanced Data,” IEEE Trans. Knowledge and Data Engineering, vol. 21, issue 9, pp. 1263-1284, 2009.](http://www.ele.uri.edu/faculty/he/PDFfiles/ImbalancedLearning.pdf)



