---
title: "Charity Funding Predictor"
---

### Background

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With my knowledge of machine learning and neural networks, I will use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, I have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

* **EIN** and **NAME**&mdash;Identification columns
* **APPLICATION_TYPE**&mdash;Alphabet Soup application type
* **AFFILIATION**&mdash;Affiliated sector of industry
* **CLASSIFICATION**&mdash;Government organization classification
* **USE_CASE**&mdash;Use case for funding
* **ORGANIZATION**&mdash;Organization type
* **STATUS**&mdash;Active status
* **INCOME_AMT**&mdash;Income classification
* **SPECIAL_CONSIDERATIONS**&mdash;Special considerations for application
* **ASK_AMT**&mdash;Funding amount requested
* **IS_SUCCESSFUL**&mdash;Was the money used effectively

### Beginning

1. Create a new repository for this project called `deep-learning-challenge`.

2. Clone the new repository to your computer.

3. Inside the local git repository, create a directory for the Deep Learning Challenge.

4. Push the above changes to GitHub.

### Instructions

### Step 1: Preprocess the Data

Using the knowledge of Pandas and scikit-learn’s `StandardScaler()`, I’ll need to preprocess the dataset. This step prepares me for Step 2, where I'll compile, train, and evaluate the neural network model.

Start by uploading the starter file to Google Colab, then using the information we provided in the Challenge files, follow the instructions to complete the preprocessing steps.

1. Read in the `charity_data.csv` to a Pandas DataFrame, and be sure to identify the following in the dataset:
  * What variable(s) are the target(s) for the model?
  * What variable(s) are the feature(s) for the model?

2. Drop the `EIN` and `NAME` columns.

3. Determine the number of unique values for each column.

4. For columns that have more than 10 unique values, determine the number of data points for each unique value.

5. Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, `Other`, and then check if the binning was successful.

6. Use `pd.get_dummies()` to encode categorical variables.

7. Split the preprocessed data into a features array, `X`, and a target array, `y`. Use these arrays and the `train_test_split` function to split the data into training and testing datasets.

8. Scale the training and testing features datasets by creating a `StandardScaler` instance, fitting it to the training data, then using the `transform` function.

### Step 2: Compile, Train, and Evaluate the Model

Using the knowledge of TensorFlow, you’ll design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset. I’ll need to think about how many inputs there are before determining the number of neurons and layers in the model. Once I’ve completed that step, you’ll compile, train, and evaluate your binary classification model to calculate the model’s loss and accuracy.

1. Continue using the file in Google Colab in which you performed the preprocessing steps from Step 1.

2. Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.

3. Create the first hidden layer and choose an appropriate activation function.

4. If necessary, add a second hidden layer with an appropriate activation function.

5. Create an output layer with an appropriate activation function.

6. Check the structure of the model.

7. Compile and train the model.

8. Create a callback that saves the model's weights every five epochs.

9. Evaluate the model using the test data to determine the loss and accuracy.

10. Save and export your results to an HDF5 file. Name the file `AlphabetSoupCharity.h5`.

### Step 3: Optimize the Model

Using the knowledge of TensorFlow, optimize the model to achieve a target predictive accuracy higher than 75%.

Use any or all of the following methods to optimize the model:

* Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
  * Dropping more or fewer columns.
  * Creating more bins for rare occurrences in columns.
  * Increasing or decreasing the number of values for each bin.
  * Add more neurons to a hidden layer.
  * Add more hidden layers.
  * Use different activation functions for the hidden layers.
  * Add or reduce the number of epochs to the training regimen.

1. Create a new Google Colab file and name it `AlphabetSoupCharity_Optimization.ipynb`.

2. Import the dependencies and read in the `charity_data.csv` to a Pandas DataFrame.

3. Preprocess the dataset as I did in Step 1. Be sure to adjust for any modifications that came out of optimizing the model.

4. Design a neural network model, and be sure to adjust for modifications that will optimize the model to achieve higher than 75% accuracy.

5. Save and export the results to an HDF5 file. Name the file `AlphabetSoupCharity_Optimization.h5`.

### Step 4: Write a Report on the Neural Network Model

The report should contain the following:

1. **Overview** of the analysis: Explain the purpose of this analysis.

2. **Results**: Using bulleted lists and images to support the answers, address the following questions:

* Data Preprocessing
  * What variable(s) are the target(s) for the model?
  * What variable(s) are the features for the model?
  * What variable(s) should be removed from the input data because they are neither targets nor features?

* Compiling, Training, and Evaluating the Model
  * How many neurons, layers, and activation functions did you select for the neural network model, and why?
  * Were I able to achieve the target model performance?
  * What steps did I take in your attempts to increase model performance?

3. **Summary**: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain my recommendation.
