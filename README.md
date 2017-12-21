# Otto product classification
Graduate course project, Introduction to Machine Learning, NYU Tandon.

**Problem statement:**

Dataset from Otto Group (one of the world’s biggest e-commerce companies) with 93 features for more than 200,000 products. The objective is to build a predictive model which is able to distinguish between its main 10 product categories .

---------------------------
## Initial Analysis of the data

The data is observed to check if all the features  are relevant for prediction. It turns out all the features are important. Tried to add variation of the original features like Sin and log on relevant features. 

---------------------------
## Try to use different Machine Learning Models with different parameters for each respective model

A table showing minimum Logloss is obtained after trying different parameters. First the models were executed normally on the the local machine. Later for generalising the models and for simplicity,  models were taken from an open source project to reduce the time in building the models. <br>
[Model_refernece Link](https://github.com/ahara/kaggle_otto/tree/master/otto/model)

| Model          | Log Loss       | 
| :---           |     :---:      |
| SVM            | 0.542290       |
| Nueral Network | 0.523256       |
| XG boost       | 0.531245       |
| Random forest  | 0.531333       |

---------------------------
## Ensemble approach to try and combine the models

Weighted average of SVM, Random forest, xgboost and nueral network was used to make prediction and the following results was obtained. The models and selected parameters selected are arbitrary. For some cases the loss did not improve.

| Model          | Log Loss       | 
| :---           |     :---:      |
| Ensemble model | 0.438593       |

---------------------------
The ensemble approach can be improved by trying different models and parameters. A comprehensive study has to be done to determine how they are exactly affecting the loss function.

Go through the wiki for detailed instructions of how to run the project. 
