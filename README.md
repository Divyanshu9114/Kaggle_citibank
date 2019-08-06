# Kaggle_citibank
Citibank Credit Defaulter prediction

Worked on Citibank dataset.

The decription of dataset given in the train1 dataset:
The description of variables:¶ Y is Client's behavior (target); 
Y=0 then not default, 
Y=1 then default. 
X1 - Amount of the given credit (NT dollar): it includes both the individual consumer credit and his/her family (supplementary) credit. 
X2 -Gender (1 = male; 2 = female). 
X3 - Education (1 = graduate school; 2 = university; 3 = high school; 0,4,5,6 = others). 
X4 - Marital status (1 = married; 2 = single; 3 = divorce; 0=others). 
X5 - Age (year). 
X6 - the repayment status in September, 2005; 
X7 - the repayment status in August, 2005 

Preprocessing:
1. Renaming the X1 - X7 column name to descriptive column name
2. Checking data in dataset and looking into data for inferences in data
3. Plot used in the dataset:
		i. Pairplot
		ii. Heatmap for finding correlation
		iii. Countplot
		iv. Scatterplot
		v. distplot
		vi. boxplot
4. Treating outlier by Interquantile method, and splitting the train data into 2, one dataset without outliers and other one with only outliers
5. Using dummification on categorical values and dropping the original columns
6. Splitting the data into train and test split
7. Using Standard Scaler to scale the data

Model Building:
1. Using predict variable using test dataset to predict for final model
2. Using Decision Tree classifier we predict the model
3. Similarly, using other model we predict the model

Post Model Building:
1. Creating model based on dataset with outliers and without outliers will give different result.
   The model created with outliers is overfitting as accuracy on train data is high but in kaggle accuracy is less.
2. Tuning the model by hyper-parameter will give better result. Decision tree and adaptive boost have highest accuracy.



Created by - Divyanshu Singh
Created on - google colab python 3 notebook and jupyter python notebook
Submitted in Kaggle, working on Citibank Predict Dafaulters
