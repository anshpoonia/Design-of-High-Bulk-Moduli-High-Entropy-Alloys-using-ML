# Design-of-High-Strength-HEAs-using-ML
This is the codebase for our research paper on High Entropy Alloy Design

The following is the tree of our repository:
```bash
.
|-- HEA_New_Folder
|   |-- Code_Notebooks
|   |   |-- Random_Validation_Test.ipynb
|   |   |-- randstate0.ipynb
|   |   |-- randstate1.ipynb
|   |   `-- randstate2.ipynb
|   |-- Datasets
|   |   |-- Classifier_sets
|   |   |   |-- random_state_0
|   |   |   |   |-- Classifier_X_test.csv
|   |   |   |   |-- Classifier_X_train.csv
|   |   |   |   |-- Classifier_y_test.csv 
|   |   |   |   `-- Classifier_y_train.csv
|   |   |   |-- random_state_1
|   |   |   |   |-- Classifier_X_test.csv 
|   |   |   |   |-- Classifier_X_train.csv
|   |   |   |   |-- Classifier_y_test.csv 
|   |   |   |   `-- Classifier_y_train.csv
|   |   |   `-- random_state_2
|   |   |       |-- Classifier_X_test.csv
|   |   |       |-- Classifier_X_train.csv
|   |   |       |-- Classifier_y_test.csv
|   |   |       `-- Classifier_y_train.csv
|   |   |-- Compositions for 10 best Bulk Modulus Values.csv
|   |   |-- Final_HEA_Classifier.csv
|   |   |-- Final_HEA_Classifier.xlsx
|   |   |-- HEA_BulkModulus.csv
|   |   |-- Regressor_sets
|   |   |   |-- random_state_0
|   |   |   |   |-- Regressor_X_test.csv
|   |   |   |   |-- Regressor_X_train.csv
|   |   |   |   |-- Regressor_y_test.csv
|   |   |   |   `-- Regressor_y_train.csv
|   |   |   |-- random_state_1
|   |   |   |   |-- Regressor_X_test.csv
|   |   |   |   |-- Regressor_X_train.csv
|   |   |   |   |-- Regressor_y_test.csv
|   |   |   |   `-- Regressor_y_train.csv
|   |   |   `-- random_state_2
|   |   |       |-- Regressor_X_test.csv
|   |   |       |-- Regressor_X_train.csv
|   |   |       |-- Regressor_y_test.csv
|   |   |       `-- Regressor_y_train.csv
|   |   |-- Scalars
|   |   |   |-- random_state_0
|   |   |   |   |-- classifier_sd_scaler.sav
|   |   |   |   `-- regressor_sd_scaler.sav
|   |   |   |-- random_state_1
|   |   |   |   |-- classifier_sd_scaler.sav
|   |   |   |   `-- regressor_sd_scaler.sav
|   |   |   `-- random_state_2
|   |   |       |-- classifier_sd_scaler.sav
|   |   |       `-- regressor_sd_scaler.sav
|   |   `-- test_32.csv
|   |-- Probability_Matrices.zip
|   |-- Saved Models
|   |   |-- Classifier Models
|   |   |   |-- random_state_0
|   |   |   |   |-- HEA_Classifier_results_dataframe.csv
|   |   |   |   |-- classifier_DecisionTree_Classifier.sav
|   |   |   |   |-- classifier_ExtraTreesClassifier.sav
|   |   |   |   |-- classifier_GaussianNB.sav
|   |   |   |   |-- classifier_NuSVC.sav
|   |   |   |   |-- classifier_SGD.sav
|   |   |   |   |-- classifier_SVC.sav
|   |   |   |   |-- classifier_XGB_Classifier.sav
|   |   |   |   |-- classifier_adaBoosting.sav
|   |   |   |   |-- classifier_gradientBoosting.sav
|   |   |   |   |-- classifier_kneighbors.sav
|   |   |   |   |-- classifier_logistic_regression.sav
|   |   |   |   `-- classifier_randomForestClassifier.sav
|   |   |   |-- random_state_1
|   |   |   |   |-- HEA_Classifier_results_dataframe.csv
|   |   |   |   |-- classifier_Adaboosting.sav
|   |   |   |   |-- classifier_DecisionTree_Classifier.sav
|   |   |   |   |-- classifier_ExtraTreesClassifier.sav
|   |   |   |   |-- classifier_GaussianNB.sav
|   |   |   |   |-- classifier_NuSVC.sav
|   |   |   |   |-- classifier_SGD.sav
|   |   |   |   |-- classifier_SVC.sav
|   |   |   |   |-- classifier_XGB_Classifier.sav
|   |   |   |   |-- classifier_gradientBoosting.sav
|   |   |   |   |-- classifier_kneighbors.sav
|   |   |   |   |-- classifier_logistic_regression.sav
|   |   |   |   `-- classifier_randomForestClassifier.sav
|   |   |   `-- random_state_2
|   |   |       |-- HEA_Classifier_results_dataframe.csv
|   |   |       |-- classifier_Adaboosting.sav
|   |   |       |-- classifier_DecisionTree_Classifier.sav
|   |   |       |-- classifier_ExtraTreesClassifier.sav
|   |   |       |-- classifier_GaussianNB.sav
|   |   |       |-- classifier_NuSVC.sav
|   |   |       |-- classifier_SGD.sav
|   |   |       |-- classifier_SVC.sav
|   |   |       |-- classifier_XGB_Classifier.sav
|   |   |       |-- classifier_gradientBoosting.sav
|   |   |       |-- classifier_kneighbors.sav
|   |   |       |-- classifier_logistic_regression.sav
|   |   |       `-- classifier_randomForestClassifier.sav
|   |   `-- Regressor Models
|   |       |-- random_state_0
|   |       |   |-- KNN_regressor.sav
|   |       |   |-- Lasso_regressor.sav
|   |       |   |-- Linear_regressor.sav
|   |       |   |-- Regression_results_dataframe.csv
|   |       |   |-- Ridge_regressor.sav
|   |       |   |-- XGBoost_regressor.sav
|   |       |   `-- random_forest_regressor.sav
|   |       |-- random_state_1
|   |       |   |-- KNN_regressor.sav
|   |       |   |-- Lasso_regressor.sav
|   |       |   |-- Linear_regressor.sav
|   |       |   |-- Regression_results_dataframe.csv
|   |       |   |-- Ridge_regressor.sav
|   |       |   |-- XGBoost_regressor.sav
|   |       |   `-- random_forest_regressor.sav
|   |       `-- random_state_2
|   |           |-- KNN_regressor.sav
|   |           |-- Lasso_regressor.sav
|   |           |-- Linear_regressor.sav
|   |           |-- Regression_results_dataframe.csv
|   |           |-- Ridge_regressor.sav
|   |           |-- XGBoost_regressor.sav
|   |           `-- random_forest_regressor.sav
|   `-- screenshots
|       |-- state0.png
|       |-- state0reg.png
|       |-- state1.png
|       |-- state1reg.png
|       |-- state2.png
|       `-- state2reg.png
`-- README.md

```

Code Notebooks consist of the notebooks that train the models and as we conducted the experiment for three different sets of train-test datasets(used random seed in train test split) each .ipynb is named based on the random seed.

The Scalars subfolder under the Datasets folder contains the copies of standard scalars used in .ipynb files

Saved Models folder contain the saved models as well as the model comparison table(as a .csv file) in their respective subfolders.

Datasets sub folder contain classifier_sets and regressor_sets which have the datasets for each of the random seeds under their respective folders.

Probability_Matrices.zip has the compressed probability matrices for elements 2-6.
