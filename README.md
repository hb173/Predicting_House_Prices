# Predicting House Prices with Machine Learning
This repository contains code for team 6's IDS 705 final project. The goal of the project is to predict house prices using housing data for [Georgia](https://www.kaggle.com/datasets/yellowj4acket/real-estate-georgia) and [California](https://www.kaggle.com/datasets/yellowj4acket/real-estate-california). All of the intial data is in the Data folder, which is all you need to run the repo. While all of our scratch work and draft files are in the the Scratch folder. All of the final versions of the files, needed to run the analysis, are in the `Code/` folder and the models are in the `models/` folder. 

## Motivation
When both buying and selling homes it is important to know the home’s price, but there are many different factors that go into it. Some of the most important factors are the different characteristics of a home. The main motivation of this project is to predict house prices of a home based on its characteristics. A pan domain analysis will first be conducted to train on homes in Georgia and California and tested by state and home type. While a within domain and cross domain analysis will be performed on each state. This will allow us to see how the different models perform on certain types of homes and their locations. It is best to get the most accurate predictions as possible, and testing on these different subsets of data will allow us to see what type of data generates the most accurate predictions. Accurate house price predictions can help sellers, buyers, and real estate agencies alike to know the market value of a home to make informed decisions. While real estate agencies and websites like Zillow could use the predicted house prices to make appropriate financial projections and advise their clientele.
 
## Data
The datasets used in this analysis are real estate data from California (CA) and Georgia (GA). They are listed from January to June 2021, and we were able to get them on Kaggle.
(https://www.kaggle.com/datasets/yellowj4acket/real-estate-georgia) and (https://www.kaggle.com/datasets/yellowj4acket/real-estate-california). 

All of the intial data is in the Data folder, which is all you need to run the repo. While all of our scratch work and draft files are in the the Scratch folder. All of the final versions of the files, needed to run the analysis, are in the Code folder and the models are in the Model folder. 


## Implementation Steps

  #### The files within the anlaysis are numerically labeled and should be run in order.
  
 - Step 1: Install the required packages via the `requirements.txt` file.
 - Step 2: First run the `Code/10_EDA&cleaning.ipynb` followed by `Code/20_Preprocessing.ipynb` to generate the needed data, which will be saved to your Data folder. 
 - Step 3: Once those files are run we were interested in testing out different possible models. The different models are in seperate notebook files whose names all start with "3x_" in the `Code/` folder. The files are each named according to the model type.
 - Step 4: The final model used was a LightGBM model. The model training code can be found in `Code/41_train_final_models.ipynb`. We trained 3 models: a model with training data from both states, and a model for with training data for each state. Trained models are saved in the `models/` folder so that you don't have to retrain the models.
 - Step 5: The final models are tested using test data in the following files: `Code/51_Validate_All_Data_Model.ipynb`(model for all of the data), `Code/52_Validating_On_California_Model.ipynb` (CA and GA on CA model), and `Code/53_Validating_On_Georgia_Model.ipynb` (CA and GA on GA model).
  
  
  ## Project Flowchart
![Picture1](https://user-images.githubusercontent.com/89568663/163626083-0a0d2de1-6439-444e-b2b7-e7f0fcd66dee.png)

![Picture2](https://user-images.githubusercontent.com/89568663/163626085-4bec457e-b86d-41e5-a53e-fa95746c92f9.png)

## Contributors
| Name | Reference |
|----|----|
|Minjung Lee| [GitHub Profile](https://github.com/minjung0)|
|Rachel Richards|[GitHub Profile](https://github.com/rjrichards27)|
|Robert Wan| [GitHub Profile](https://github.com/rw417)|
|Himangshu Raj Bhantana | [GitHub Profile](https://github.com/hb173)|
