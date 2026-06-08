<div id="bootcamp"><img style="display: none;" src="https://static.bc-edx.com/data/dl-1-2/m21/lms/img/banner.jpg" alt="lesson banner" />

# Nonprofit Funding Success Prediction Using Deep Learning

## Overview

This project applies deep learning techniques to predict whether nonprofit organizations are likely to successfully utilize funding resources based on historical application and organizational data.

Using a dataset containing over 34,000 funded organizations, a neural network classification model was developed to identify patterns associated with successful funding outcomes. The project demonstrates how machine learning can support data-driven funding decisions and improve resource allocation strategies for nonprofit foundations.

The workflow includes data preprocessing, feature engineering, neural network development, model optimization, and performance evaluation.

---

# Project Objectives

The primary goals of this project are to:

* Predict the likelihood of nonprofit funding success
* Identify organizational characteristics associated with successful outcomes
* Develop and optimize a deep learning classification model
* Compare model performance across multiple neural network architectures
* Evaluate predictive accuracy using industry-standard metrics
* Demonstrate practical applications of deep learning in decision-making processes

---

# Dataset

The dataset contains historical records of organizations that previously received funding from a nonprofit foundation.

Features include:

* Application type
* Industry affiliation
* Organizational classification
* Funding use case
* Organization type
* Operational status
* Income classification
* Special considerations
* Funding amount requested

The target variable indicates whether the funded organization achieved a successful outcome.

### Target Variable

* **IS_SUCCESSFUL**

  * 1 = Successful Outcome
  * 0 = Unsuccessful Outcome

---

# Analysis & Methodology

## Data Preparation

Prepared the dataset for machine learning by:

* Removing non-predictive identifier fields
* Handling categorical variables
* Grouping rare categories
* Applying one-hot encoding
* Splitting training and testing datasets
* Scaling numerical features

These preprocessing steps improved model performance and training efficiency.

---

## Neural Network Development

Built a binary classification model using TensorFlow and Keras.

The model architecture included:

* Input layer
* Hidden layers
* Output layer
* Nonlinear activation functions

The network was designed to learn complex relationships between organizational characteristics and funding outcomes.

---

## Model Training & Evaluation

The neural network was trained on historical funding records and evaluated using unseen test data.

Performance metrics included:

* Accuracy
* Loss
* Precision
* Recall
* Classification performance

These metrics help assess the model’s ability to distinguish between successful and unsuccessful funding outcomes.

---

## Model Optimization

Multiple optimization strategies were explored to improve predictive performance.

Techniques included:

* Adjusting hidden layer structures
* Modifying neuron counts
* Testing alternative activation functions
* Experimenting with training epochs
* Refining categorical feature grouping

Several model iterations were compared to identify the most effective architecture.

---

## Predictive Funding Analysis

The final model can be used as a decision-support tool for evaluating future funding applications.

Potential use cases include:

* Applicant screening
* Funding prioritization
* Resource allocation
* Risk reduction
* Program effectiveness assessment

---

# Technologies Used

* Python
* Pandas
* NumPy
* TensorFlow
* Keras
* Scikit-Learn
* Google Colab
* Jupyter Notebook

---

# Key Skills Demonstrated

This project demonstrates experience with:

* Deep learning
* Neural network architecture design
* Binary classification
* Feature engineering
* Data preprocessing
* Model optimization
* Hyperparameter tuning
* TensorFlow and Keras development
* Predictive analytics
* Applied machine learning

---

# Key Insights

Major findings from the analysis include:

* Organizational characteristics contain meaningful signals associated with funding success.
* Deep learning models can effectively capture nonlinear relationships within nonprofit funding data.
* Feature preprocessing and category consolidation significantly influence model performance.
* Model optimization can improve predictive accuracy beyond baseline neural network architectures.
* Predictive analytics can support more efficient and evidence-based funding decisions.

---

# Business Impact

Accurately predicting funding outcomes can help nonprofit organizations and grant-making institutions:

* Improve allocation of limited funding resources
* Increase the probability of successful project outcomes
* Reduce funding inefficiencies
* Support evidence-based decision making
* Enhance long-term program effectiveness

This project demonstrates how deep learning can transform historical organizational data into actionable funding intelligence.

---

# Disclaimer

This project was completed for educational and portfolio purposes.

The dataset is used to demonstrate deep learning, predictive analytics, and nonprofit funding classification techniques.
