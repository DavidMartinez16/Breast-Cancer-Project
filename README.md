# Breast Cancer Estimator: Project Overview

_This is a data science project that uses the breast cancer dataset, the objective is to predict the diagnosis by analyzing features of the tumor such as area, perimeter, radius, smoothness, compactness, concavity, symmetry, texture, etc_


* Created a tool that estimates whether a tumor is malignant of benign by analyzing different features of itself
* [Dataset](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data) - The used dataset was downloaded from the kaggle repository
* Models such as Logistic Regression, Support Vector Machines, K-Nearest Neighbors and Decision Trees obtained the best performance, with accuracy values greater than 90 % and F1-score greater than 93 %

## Code and Resources Used 🛠️

* **Python Version:** 3.7
* **Packages:** Pandas, Numpy, Matplotlib, Seaborn, Sklearn and Scikitplot

## Features of the data 📦
_The following are the features contained in the Breast Cancer Wisconsin Dataset :_

* Id                      
* Diagnosis                
* Radius_mean              
* Texture_mean             
* Perimeter_mean           
* Area_mean                
* Smoothness_mean        
* Compactness_mean         
* Concavity_mean           
* Concave points_mean      
* Symmetry_mean            
* Fractal_dimension_mean   
* Radius_se                
* Texture_se               
* Perimeter_se            
* Area_se                 
* Smoothness_se         
* Compactness_se       
* Concavity_se
* Concave points_se        
* Symmetry_se              
* Fractal_dimension_se     
* Radius_worst             
* Texture_worst            
* Perimeter_worst          
* Area_worst               
* Smoothness_worst         
* Compactness_worst       
* Concavity_worst         
* Concave points_worst    
* Symmetry_worst          
* Fractal_dimension_worst  4
* Unnamed: 32  

## Data Cleaning

* Drop the Id and the Unnamed: 32 columns, do not provide useful information
* Replace the categorical values of diagnosis such as ('M' - Malignant) and ('B' - Benign) to numerical values such as 0 and 1 respectively
* Scale the values in the columns to a range of 0 to 100 in order to balance the data
* Finally, save the processed data

## Some Exploratory Data Analysis (EDA)

_Verify the correlation between the features with the diagnosis_

![Corrrelations](https://user-images.githubusercontent.com/63115543/91640801-c9c2f080-e9e5-11ea-9bf3-816049f4d749.jpg)

_Plot scatters of differente features_

![scat](https://user-images.githubusercontent.com/63115543/91640877-58d00880-e9e6-11ea-9aaa-6b8255341b6c.jpg)

## Model Building

First, i split the data into train and test sets with a test size of 20 %. Then i tried four different models and evaluated them using the score function.

The models i tried are the following :
* Logistic Regression
* Support Vector Machines
* K-Nearest Neighbors
* Decision Trees

## Performance 

### Logistic Regression
* F1 Score : 0.9824561403508771 
* Accuracy : 0.9824561403508771 
* Sensibility : 0.9523809523809523 
* Specifity : 1.0

### Support Vector Machines
* F1 Score : 0.956140350877193 
* Accuracy : 0.956140350877193 
* Sensibility : 0.8809523809523809 
* Specifity : 1.0 

### K-Nearest Neighbors
* F1 Score : 0.9385964912280702 
* Accuracy : 0.9385964912280701 
* Sensibility : 0.8571428571428571 
* Specifity : 0.9861111111111111 

### Decision Trees
* F1 Score : 0.9473684210526315 
* Accuracy : 0.9473684210526315 
* Sensibility : 0.9047619047619048 
* Specifity : 0.9722222222222221 

_As you can see, the model with the best performance is the Logistic Regression, following the confusion matrix and the ROC Curve of this model_


