## Overview

The nonprofit organization Alphabet Soup aims to develop an algorithm for predicting the success of funding applicants.
Leveraging machine learning and neural network expertise, our goal is to utilize the features within the provided dataset to construct a binary classifier capable of forecasting whether applicants will achieve success when sponsored by Alphabet Soup.

## Results

### Data Preprocessing

To initiate the data processing, we first eliminated any irrelevant information. After excluding **"EIN"** and **"NAME"**, the remaining columns were designated as features for our model. **"NAME"** was subsequently reintroduced in the second phase for binning purposes.
The data was then divided into training and testing sets. The target variable for our model was labeled **"IS_SUCCESSFUL"**, taking the value **1** for "yes" and **0** for "no."
We conducted an analysis of the **APPLICATION** data, with a focus on the **"CLASSIFICATION"** variable for binning purposes. We established specific data thresholds to group together **"rare"** variables and assigned a new label of **"Other"** for each unique value falling below these thresholds.
Categorical variables were encoded using the **get_dummies()** method after confirming the success of the binning process.

### Compile, Train and Evaluate the Model

Each model, after applying neural networks, consisted of a total of three layers. 
The number of hidden nodes was determined by the number of features.

![image](https://github.com/jhyang13/ds_bootcamp_module21/assets/98197333/a85ad66c-ef8b-48c0-9797-f572e358c8bc)

A three-layer training model generated 477 parameters. 
The initial attempt achieved slightly over 73% accuracy, which fell slightly short of the desired 75% but was still fairly close.

![image](https://github.com/jhyang13/ds_bootcamp_module21/assets/98197333/dfb85cf4-f008-4f77-b63e-b3c6195c8f23)

### Optimize the Model

