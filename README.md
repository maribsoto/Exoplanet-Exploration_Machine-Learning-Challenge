# Exoplanet Exploration
## Machine Learning Challenge

![exoplanets.jpg](images/exoplanets.jpg)

## Background & Scope
 
For more than nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.
To help process this data, I created 2 machine learning models capable of classifying candidate exoplanets from the raw dataset.
I followed the following steps:

    * Preprocess the raw data
    * Tune the models
    * Compare two or more models

### Data sources
* https://www.kaggle.com/nasa/kepler-exoplanet-search-results
* https://exoplanetarchive.ipac.caltech.edu/docs/API_kepcandidate_columns.html

## Screenshots from data pre-processing and tuning

### Principal Components Analysis

![corr_coeff.png](images/corr_coeff.png)

### Pairplot Displays

![pairplot.png](images/pairplot.png)

## Model 1: Logistic Regression 

### Classification Report
![LR_classif_rep.png](images/LR_classif_rep.png)

### Model Results: KOI Disposition Actual vs. Predicted
![LR_pred_results.png](images/LR_pred_results.png)

### Best scores for the current model
![LR_best_score](images/LR_best_score.png)

## Model 2: K Nearest Neighbors 

### Classification Report
![knn_classif_rep.png](images/knn_classif_rep.png)

### KNN Plot
![knn_plot](images/knn_plot.png)

### Best scores for the current model
![knn_best_score](images/knn_best_score.png)


## Models Comparison and Findings

Current results of the Logistic Regression and KNN models have scores of 0.61 and 0.63, respectively. The KNN model is slightly more accurate than LR. 

PAC table show that the data set correlation coefficients among variables vary considerably. In some cases, coefficients are very low or non existant.  

Some PairPlot displays are very sparse. The less sparse plots were selected.

A more thorough review of the available dataset may through better model scores. Even more, other statistical approaches such as Random Forest or SVM, may produce more accurate results.