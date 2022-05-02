# Car price Estimator:Project Overview
* Created a tool that estimates Car price (MAE ~ $ 1334 ) to help car owners  to calculate value of their car for    selling.
* Performed **EDA** and **feature enginnering** on dataset.
* Analyzed categorical features which were converted to numerical later.
* Optimized Random Forest Regressors using RandomsearchCV **(Hyperparameters tuning)** to reach the best model.

## Packages used:
* pandas, numpy, sklearn, matplotlib, seaborn,pickle.

## Data Cleaning
* Removed some columns which might not be use full.
* 10 Categorical features  were converted to numerical so that it was usable for our model.

## EDA 
* I looked at the distributions of the data and the value counts for the various variables.Below are a few highlights
 ![image](https://user-images.githubusercontent.com/88432965/166185598-a435dcec-a10b-450f-b4f7-85e59614d5fa.png)
 ![image](https://user-images.githubusercontent.com/88432965/166185538-1c115911-45cc-45b0-9d28-c4759b01c5b4.png)
 
* Here the maximum fueltype is gas and the cars with fuel type diesel are more costly
1. first graph shows car counts with maximum fuel type.
2. Second graph shows price of car depending on fuel.

![image](https://user-images.githubusercontent.com/88432965/166185714-cbc154f8-0618-41a0-b4da-42b9afe817ac.png)
* The most selled cars are sedan and least ones are convertable.
* 
### 5 Important Features 
![image](https://user-images.githubusercontent.com/88432965/166185848-5b4d5f81-3b32-40d0-bc6f-780aa49b1cdf.png)

## Model Building
* First I mapped Categorical values with numerical values. Used RandomizedSearchCV to find the best parameters for model training.
* Split the data into train and tests sets with a test size of 30%.
* Used StandardScaler to scale the data.

## Model performance

Score: 90% 

MAE: 1334.688791794163


