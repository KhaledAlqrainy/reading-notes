# Machine Learning Intro

## Bird's Eye View

### Machine learning is a comprehensive approach to solving problems and it can be divided into:

- exploratory analysis by first, "get to know" the data
- data cleaning by cleaning your data to avoid many common pitfalls
- feature engineering by helping your algorithms "focus" on what's important by creating new features
- algorithm selection by Choosing the best algorithms
- model training by training your models


### In machine learning we are practicing of teaching computers how to learn patterns from data and decisions or predictions. in applied machine learning, you pick first the right machine learning task for the job where a task is a specific objective for your algorithms. there are two common categories of tasks and they are:

- Supervised Learning which use:
    - Regression 
    - Classification
- Unsupervised Learning which use:
    - Clustering


## Exploratory Analysis

> Exploratory analysis is about answering questions and extracting enough insights from your dataset. it should be quick, efficient, and decisive. to understand and visualize the dataset we can use:


- Plot Numerical Distributions like histograms which is enough to understand the dataset distributions
- Plot Categorical Distributions like bar plots
- Plot Segmentations like Box plots 


* After data visualization we can study correlations as positive, negative, strong relationship, weak relationship , and no relationship


## Data Cleaning

### cleaning data is about:

- Removing unwanted observations which includes:
    - Duplicate observations
    - Irrelevant observations
- Fix Structural Errors
- Filter Unwanted Outliers
- Handle Missing Data like:
    - Missing categorical data
    - Missing numeric data


## Feature Engineering

> Feature engineering is about creating new input features from your existing ones by infuse domain knowledge, create interaction features, combine sparse classes, add dummy variables and remove unused features.


## Algorithm Selection

* Individual algorithms should be swapped in and out depending on which performs best for the problem and the dataset


### Linear regression models are very common. it fit a straight line. its main advantage is that they are easy to interpret and understand. simple linear regression suffers from two major flaws:

- It's prone to over fit with many input features.
- It cannot easily express non-linear relationships.

## Model Training

### model training starts by splitting dataset into:

- Train set
- Test set

* Training set are used to fit and tune your models. Test set are put aside as unseen data to evaluate your models. tuning models means tuning hyperparameter which express higher-level structural settings for algorithms

* To fit and tune our models we perform the entire cross-validation loop detailed above on each set of hyperparameter values we'd like to try

* Cross-validation is a method for getting a reliable estimate of model performance using only your training data