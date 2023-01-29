# 64hour-ML-hackathon

Overview
This document summarises the analysis and training of a RandomForest model applied to the device_failure.csv dataset and is complementary to the jupyter notebook that contains the code and algorithms used to achieve the results presented in this document. Question You are tasked with building a model using machine learning to predict the probability of a device failure. When building this model, be sure to minimize false positives and false negatives. The column you are trying to predict is called failure with binary value 0 for non-failure and 1 for failure.

The Dataset
The dataset was composed 12 columns: date, device, failure, and attribute[1-9] and it has a total of 124494 rows of records from 2015-01-01 to 2015-11-02 for a total of 304 days of records. The device column has 1163 unique classes, and the target column failure has two classes ‘0’ and ‘1’.

Implementation
For the implementation, firstly the data is clustered by dates and devices, secondly the exploratory data analysis starts by calculating the rates for failure, survival and replacement are calculated. Next, the columns are inspectioned to assess similarities within each other. After the inspection, all the columns values are plotted for 12 randomly picked devices to assess the differences and correlations between variables. After the EDA, the dataset is transformed to drop columns and rows that are not relevant for the modelling, and also created new features for the dataset. Finally, after the dataset is cleaned and enhanced, the dataset is passed through a RandomForest model, the confusion matrix is calculated and the model evaluated and compared with its baseline.

Conclusions
In order to produce better results, further investigation and EDA needs to be done, as well as to produce accurate results, is necessary to dive deeper into the relationships of the attributes with the failure, as well as collect better data of the device’s failures. With more data, the algorithm will be able to produce better results and avoid the overfitting of the model due to the imbalance of the dataset.
