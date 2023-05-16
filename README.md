# Diabetic Retinopathy Detection using CNN

<div align="center">
  <img src="https://github.com/Piyush42Soni/Diabetic-Retinopathy-Detection-using-CNN/blob/main/Eye_AI.png" width=250 />
  
  ![Python](https://img.shields.io/badge/Python-4FDEEE.svg?style=for-the-badge&logo=python&logoColor=white)
  ![Tensorflow](https://img.shields.io/badge/tensorflow-%23F24E1E.svg?style=for-the-badge&logo=tensorflow&logoColor=white)
  ![Scikit Learn](https://img.shields.io/badge/scikit_Learn-%FFBF00.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
  ![Numpy](https://img.shields.io/badge/numpy-332690.svg?style=for-the-badge&logo=numpy&logoColor=white)
</div>

## Problem Description
Diabetic retinopathy is an eye condition that can cause vision loss and blindness in people who have diabetes. It affects blood vessels in the retina (the light-sensitive layer of tissue in the back of your eye). If someone have diabetes, it’s important to get a comprehensive dilated eye exam at least once a year.

DR Severity Level | Lesions 
--- | --- 
No DR |	Absent of lesions
Mild non-proliferative DR |	MA only
Moderate non-proliferative DR |	(More than just MA but less than severe DR
Severe non-proliferative DR	Any of the following: | more than 20 intraretinal HM in each of 4 quadrants, definite venous beading in 2+ quadrants, prominent intraretinal microvascular abnormalities in 1+ quadrant and no signs of proliferative DR)

## Task
Predict whether diabetic retinopathy is referenceable (NPDR {Moderate or beyond} or DPR with NDE) or not.

## Model

I have created a deep learning model that uses the **CNN model** for the binary classification of diabetic retinopathy. Here are the results generated (average of 10 trials) :
1. The average **accuracy of the model is 98.04%.**
2. f1 score of 0.985
3. The precision for output 1 is 1.00.
4. The precision for output 0 is 0.97.
5. recall for output 0 is 1.00
6. The recall for output 1 is 0.97.
7. **sensitivity is 1**
 
I have observed that the data was imbalanced; therefore, I have used oversampling using **SMOTE** to make the data balanced in both cases. Also, I have used data **augmentation and normalization** for better training of the model and to prevent overfitting. I have used the **Adam optimization technique** and the **binary cross-entropy loss function.**
 
Then I have compared my CNN model with an ANN and a Naive Bayesian model, and here are the results:
 
ANN Model
I have used SMOTE oversampling, data augmentation, and data normalization, but it does not affect the results of ANN.
1. Accuracy is 50%.
2. The sensitivity is 0.
 
Naive Bayesian Model
1. The average accuracy of test data is 60%.
2. f1 score of 0.57
  
  ### Model Structure
  
  <div align="center">
  <img src="https://github.com/Piyush42Soni/Diabetic-Retinopathy-Detection-using-CNN/blob/main/model_structure.png" width=250/>
  </div>
  
  ### Model ROC curve
  <img src="https://github.com/Piyush42Soni/Diabetic-Retinopathy-Detection-using-CNN/blob/main/ROC_curve_for_CNN.png" width=300 />
  
  ### Model confusion matrix
  <img src="https://github.com/Piyush42Soni/Diabetic-Retinopathy-Detection-using-CNN/blob/main/confusion%20_matrix_for_CNN.png" width=300 />
  
## **Conclusion: CNN models are better than ANN and the Naive Bayesian Model for binary classification.**
