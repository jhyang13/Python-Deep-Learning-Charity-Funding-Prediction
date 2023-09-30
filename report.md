## Overview

The nonprofit organization Alphabet Soup aims to develop an algorithm for predicting the success of funding applicants.
Leveraging machine learning and neural network expertise, our goal is to utilize the features within the provided dataset to construct a binary classifier capable of forecasting whether applicants will achieve success when sponsored by Alphabet Soup.

## Results

### Data Preprocessing

To initiate the data processing, we first eliminated any irrelevant information. After excluding **EIN** and **NAME**, the remaining columns were designated as features for our model. **NAME** was subsequently reintroduced in the second phase for binning purposes.
The data was then divided into training and testing sets. The target variable for our model was labeled **"IS_SUCCESSFUL"**, taking the value **1** for "yes" and **0** for "no."
We conducted an analysis of the **APPLICATION** data, with a focus on the **"CLASSIFICATION"** variable for binning purposes. We established specific data thresholds to group together **"rare"** variables and assigned a new label of **"other"** for each unique value falling below these thresholds.
Categorical variables were encoded using the **get_dummies()** method after confirming the success of the binning process.

