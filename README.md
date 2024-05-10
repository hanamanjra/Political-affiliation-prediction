# Political-affiliation-prediction

We will be using the following dataset published by Dr Stuart Bramwell:

Nyrup, Jacob, Hikaru Yamagishi, and Stuart Bramwell. 2023a. “Replication Data for: Consolidating Progress: The Selection of Female Ministers in Autocracies and Democracies.” Harvard Dataverse, v1 


This project involves two main analyses: the investigation of regime changes between autocracy and democracy at the country level and the examination of the increase in female ministers in cabinet positions.

#Regime Change Analysis

The regime change analysis focuses on understanding transitions between autocratic and democratic systems at the country level. This involves examining historical data to identify instances where a country's political regime shifts from autocracy to democracy or vice versa.

#Female Minister Representation Analysis

The analysis of the increase in female ministers in cabinet positions begins by creating a binary target variable, 'is_share_female_up', indicating a 10% increase in female representation compared to the previous year. Two baseline logistic regression models are developed, utilizing a female empowerment index and the share of women in high positions as predictors. Separate training and testing sets are created for each model, with performance evaluated using AUC values. Threshold testing is conducted to optimize precision and recall balance. Time-series cross-validation with a rolling-window resample (381 iterations) assesses model stability and generalization. Feature engineering involves constructing a multiple logistic regression incorporating various predictors, such as time lagged variables and proportions of high and low female ministers, with an analysis of each predictor's incremental contribution to predicting increased female minister representation.
