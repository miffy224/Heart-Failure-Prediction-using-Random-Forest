# Heart-Failure-Prediction-using-Random-Forest
There are some factors that affects Death Event. This dataset contains person's information like age ,sex , blood pressure, smoke, diabetes, ejection fraction, creatinine phosphokinase, serum_creatinine, serum_sodium, time and we have to predict their DEATH EVENT.


# Data Source
[Heart Failure Prediction](https://www.kaggle.com/andrewmvd/heart-failure-clinical-data)


# Data Processing
This dataset is only 299 rows, which is not a very large dataset to train or
test on. So to be fair to both training and testing, I split the data into 50%
train and 50% test.
In addition, the data is originally uneven distributed respect to “DEATH
EVENT”. So, I rearranged the data sequence in random order to let both train
and test data have a close death rate.

# Prediction Target
There are some factors that affects Death Event. This dataset contains
person's information like age, sex, blood pressure, smoke, diabetes, ejection
fraction, creatinine phosphokinase, serum_creatinine, serum_sodium, time
and we have to predict their DEATH EVENT.


￼![image](https://user-images.githubusercontent.com/18226575/111269241-af92ec00-8671-11eb-8d49-799bbbe5b252.png)

# Background
Heart failure is a common event caused by cardiovascular diseases and this  dataset contains 12 features that can be used to predict mortality by heart  failure. 
People with cardiovascular disease or who are at high cardiovascular risk  need early detection and management where in a machine learning model  can be of great help. 

# ⽤いた⼿法の簡潔な説明（Methods）： 
1. Random Forest 
2. Random Forest With PCA Reduced Dimensionality 
3. Random Forest With PCA Reduced Dimensionality & Hyper-parameter  Tuning 

## テストデータに対する予測精度（Accuracy）： 
### ```RF > RF+PCA+Hyper-parameter > RF+PCA ```

1. Accuracy of Random Forest: 0.756 

|               | predicted 0   | predicted 1  |
| ------------- |:-------------:| -----:|
| actual 0      | 96            | 9     |
| actual 1      | 11            | 34    |

2. Accuracy of Random Forest With PCA: 0.467 

|               | predicted 0   | predicted 1  |
| ------------- |:-------------:| -----:|
| actual 0      | 95            | 10     |
| actual 1      | 24            | 21    |

3. Accuracy of Random Forest With PCA & Hyper-parameter: 0.489

|               | predicted 0   | predicted 1  |
| ------------- |:-------------:| -----:|
| actual 0      | 95            | 10     |
| actual 1      | 23            | 22    |


Looking at the picture below, when we use PCA to reduce the 12  predicting variables down to 10 components, we can explain over 95% of  the variance.

￼![image](https://user-images.githubusercontent.com/18226575/111270570-60e65180-8673-11eb-8b3b-86fa7700fb4b.png)





