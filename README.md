<h2><P align=center> Credit_Risk_Analysis </p></h2>

<h3><P align=center> Overview Of The Analysis </p></h3>

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, this analysis takes the approach of employing different techniques to train and evaluate models with unbalanced classes. The imbalanced-learn and scikit-learn libraries are used to build and evaluate models with resampling in this analysis.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data is oversampled using the RandomOverSampler and SMOTE algorithms. This is followed by the undersampling of the data using the ClusterCentroids algorithm, combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, the two new machine learning models that reduce bias are compared against each other, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

<h2><P align=center>  Results </p></h2>
<br>
<h3> Let us look at the balanced accuracy scores, precision and recall scores of all six machine learning models one by one.  </h3>
<br>
<h3><P align=center> 1. Naive Random Oversampling</p> </h3>
<br> 

<kbd>
<img width="804" alt="Screen Shot 2022-02-27 at 4 32 34 PM" src="https://user-images.githubusercontent.com/90424752/155906924-f7ea7080-4e66-4d6a-a707-a26ffbe107a6.png">


</kbd>

- Precision Score : 0.01 (high_risk) & 1.00 (low_risk)
- Accuracy of the Classifier : 67.42%
- Recall : 0.74 (high_risk) & 0.61 (low_risk)
- F1 score : 0.02 (high_risk) & 0.67 (low_risk)


<h3><P align=center>2. SMOTE Oversampling </p> </h3>
<br> 

<kbd>
<img width="805" alt="Screen Shot 2022-02-27 at 4 33 07 PM" src="https://user-images.githubusercontent.com/90424752/155906944-5caf3ff2-116e-4118-ad9e-f427a54c1c53.png">


</kbd>

- Precision Score : 0.01 (high_risk) & 1.00 (low_risk)
- Accuracy of the Classifier : 66.23%
- Recall : 0.63 (high_risk) & 0.69 (low_risk)
- F1 score : 0.02 (high_risk) & 0.82 (low_risk)

<h3><P align=center>3. Cluster Centroids Resampling </p> </h3>
<br> 

<kbd><img width="805" alt="Screen Shot 2022-02-27 at 4 13 03 PM" src="https://user-images.githubusercontent.com/90424752/155906189-281c4a1b-3587-464e-9c75-462f3c00f8d2.png"></kbd>



- Precision Score : 0.01 (high_risk) & 1.00 (low_risk)
- Accuracy of the Classifier : 54.47%
- Recall : 0.69 (high_risk) & 0.40 (low_risk)
- F1 score : 0.01 (high_risk) & 0.57 (low_risk)


<h3><P align=center>4. SMOTEEN Resampling </p> </h3>
<br> 

<kbd>

<img width="806" alt="Screen Shot 2022-02-27 at 4 36 55 PM" src="https://user-images.githubusercontent.com/90424752/155907093-d72933d9-0d92-43bc-afbb-cb449b2125c8.png">


</kbd>

- Precision Score : 0.01 (high_risk) & 1.00 (low_risk)
- Accuracy of the Classifier : 64.00%
- Recall : 0.70 (high_risk) & 0.58 (low_risk)
- F1 score : 0.02 (high_risk) & 0.73 (low_risk)


<h3><P align=center>5. Balanced Random Forest Classifier </p> </h3>
<br> 

<kbd>

  <img width="804" alt="Screen Shot 2022-02-27 at 4 40 02 PM" src="https://user-images.githubusercontent.com/90424752/155907264-37e3e94e-baf3-4ecf-8477-0915de4f7f93.png">


</kbd>


- Precision Score : 0.03 (high_risk) & 1.00 (low_risk)
- Accuracy of the Classifier : 78.85%
- Recall : 0.70 (high_risk) & 0.87 (low_risk)
- F1 score : 0.06 (high_risk) & 0.93 (low_risk)


<h3><P align=center>6. Easy Ensemble AdaBoost Classifier </p> </h3>
<br> 

<kbd>

<img width="805" alt="Screen Shot 2022-02-27 at 4 40 38 PM" src="https://user-images.githubusercontent.com/90424752/155907286-32dad71a-ca67-4eac-8971-e8406652c359.png">


</kbd>

- Precision Score : 0.09 (high_risk) & 1.00 (low_risk)
- Accuracy of the Classifier : 93.16%
- Recall : 0.92 (high_risk) & 0.94 (low_risk)
- F1 score : 0.16 (high_risk) & 0.97 (low_risk)




<h2><P align=center>  Summary </p></h2>


<h4> Recommendations </h4>

