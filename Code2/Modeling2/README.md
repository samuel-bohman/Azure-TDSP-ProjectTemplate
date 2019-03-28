# Modeling and Related Activities

## Goals

* Determine the optimal data features for the model.  
* Create an informative model that predicts the target most accurately.  
* Create a model that's suitable for production.  

## How to do it

There are three main tasks addressed in this stage:

* **Feature engineering**: Create data features from the raw (cleaned) data to facilitate model training.
* **Model training**: Find the model that answers the question most accurately by comparing their success metrics.
* Determine if your model is **suitable for production**.

### Feature engineering

Feature engineering involves the inclusion, aggregation, and transformation of raw variables to create the features used in the analysis. This step requires a creative combination of domain expertise and the insights obtained from the data exploration step. 

### Model training

The process for model training typically includes the following steps:

* Split the input data (randomly) for modeling into a training set and a test set.
* Build the models by using the training set.
* Evaluate the training and the test set. Use a series of competing algorithms along with the various associated tuning parameters (known as a parameter sweep) that are geared toward answering the question of interest with the current data.  
* Determine the “best” solution to answer the question by comparing the success metrics between alternative methods.

The TDSP provide an automated modeling and reporting tool that's able to run through multiple algorithms and parameter sweeps to produce a baseline model. It also produces a baseline modeling report that summarizes the performance of each model and parameter combination including variable importance. This process is also iterative as it can drive further feature engineering.

## Artifacts

The artifacts produced in this stage include:

* **Feature sets**: The features developed for the modeling are described in the **Feature sets** section of the **Data definition** report. It contains pointers to the code to generate the features and a description of how the feature was generated.  
* **Model report**: For each model that's tried, a standard, template-based report that provides details on each experiment is produced.  
* **Checkpoint decision**: Evaluate whether the model performs well enough to deploy it to a production system. Some key questions to ask are:
    * Does the model answer the question with sufficient confidence given the test data?  
    * Should you try any alternative approaches? Should you collect additional data, do more feature engineering, or experiment with other algorithms?  
  
## Next step

The next step in the lifecycle of the TDSP is **Deployment**. 

## Further reading

This guideline is an excerpt from the [Team Data Science Process documentation](https://docs.microsoft.com/en-us/azure/machine-learning/team-data-science-process/lifecycle-modeling)
