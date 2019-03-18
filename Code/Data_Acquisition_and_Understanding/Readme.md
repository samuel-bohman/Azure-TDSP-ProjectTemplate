# Data Acquisition and Understanding

## Goals

* Produce a clean, high-quality data set whose relationship to the target variables is understood. Locate the data set in the appropriate analytics environment so you are ready to model.
* Develop a solution architecture of the data pipeline that refreshes and scores the data regularly.

## How to do it

There are three main tasks addressed in this stage:

* **Ingest the data** into the target analytic environment.
* **Explore the data** to determine if the data quality is adequate to answer the question.
* **Set up a data pipeline** to score new or regularly refreshed data.

### Ingest the data

Set up the process to move the data from the source locations to the target locations where you run analytics operations, like training and predictions.

### Explore the data

Before you train your models, you need to develop a sound understanding of the data. Real-world data sets are often noisy, are missing values, or have a host of other discrepancies. You can use data summarization and visualization to audit the quality of your data and provide the information you need to process the data before it's ready for modeling. This process is often iterative.

TDSP provides an automated utility, called IDEAR, to help visualize the data and prepare data summary reports. We recommend that you start with IDEAR first to explore the data to help develop initial data understanding interactively with no coding. Then you can write custom code for data exploration and visualization.

After you're satisfied with the quality of the cleansed data, the next step is to better understand the patterns that are inherent in the data. Again, this process is often iterative. 

### Set up a data pipeline

In addition to the initial ingestion and cleaning of the data, you typically need to set up a process to score new data or refresh the data regularly as part of an ongoing learning process. You do this by setting up a data pipeline or workflow. In this stage, you develop a solution architecture of the data pipeline. You develop the pipeline in parallel with the next stage of the data science project. Depending on your business needs and the constraints of your existing systems into which this solution is being integrated, the pipeline can be one of the following:

* Batch-based
* Streaming or real time
* A hybrid

## Artifacts

The following are the deliverables in this stage:

* **Data summary report**: This report includes data summaries, the relationships between each attribute and target, variable ranking, and more. The IDEAR tool provided as part of TDSP can quickly generate this report on any tabular data set, such as a CSV file or a relational table.  
* **Solution architecture**: The solution architecture can be a diagram or description of your data pipeline that you use to run scoring or predictions on new data after you have built a model. It also contains the pipeline to retrain your model based on new data. Store the document in the Project directory when you use the TDSP directory structure template. 
* **Checkpoint decision**: Before you begin full-feature engineering and model building, you can reevaluate the project to determine whether the value expected is sufficient to continue pursuing it. You might, for example, be ready to proceed, need to collect more data, or abandon the project as the data does not exist to answer the question.  

## Next step

The next step in the lifecycle of the TDSP is **Modeling**. 

## Further reading

This guideline is an excerpt from the [Team Data Science Process documentation](https://docs.microsoft.com/en-us/azure/machine-learning/team-data-science-process/lifecycle-data)
