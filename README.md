# Optimized-Ensemble-Prediction-Model-for-Breast-Cancer

link to the publication - https://ieeexplore.ieee.org/document/9615269
1. Introduction - Ensemble learning, Stack Generalization
2. Project Description
    a) Instances and the applied work
    b) Attributes and the applied work
    c) Model Building
    d) Result and Conclusion
-------------------------------------------
    1. Ensemble Learning is the combination of algorithms, and nowadays with machine learning, it has taken its own pace in prediction which has proved to be beneficial in health care sector, trading sector and various corporate sector in evaluating the overall efficiency of the personnel and machines or any use-case. There are basically 3 types of  ensemble learning: Bagging, Boosting and Stacking or Stack Generalization. In this project I have developed an Stacking model which combines the predictions of the base level algorithms as input vectors to the meta learner and makes a better prediction by inculcating the performance of the various algorithms. 
------------------------------------------- 
    2. Breast cancer is the 2nd most dangerous of all cancers in women.
Data set used in this project- WBDC(https://archive.ics.uci.edu/ml/datasets/breast+cancer+wisconsin+(diagnostic))

     a) Instances- 569 out of which 70% is used for building the model with cross validation - 5 and 30% is used for testing the model.
  
     b) Attributes(32) - With Pearson Correlation Coefficient we found the best attributes - 10 attributes and Normalised the data with Z-score Normalization and removed the outliers with Local-Outlier-Factor an unsupervised machine learning technique to detect the outliers.

     c) Model Building - Various predictions of different algorithms are chosen here(Support vector classifier, Multilayer Perceptron, K Nearest Neighbour and Random Forest) and the predictions are passed as input to the final model( Gaussian Naive Bayes).

(SVC + MLP + KNN + RF)------->predictions from the 4 algorithms are given as input---------->Gaussian Naive Bayes------->which makes the final prediction

     d) The stacked model has successfully classified 568 instances out of 1 misclassified instance. The conclusion drawn from 99.41% is that it surpasses various works on the same dataset with machine learning and it is a stacked ensemble model with lot of possibilities in the near future.