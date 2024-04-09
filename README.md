# SnowparkHOL_April24

Overview
By completing this guide, you will be able to go from raw data to an interactive application that can help organization optimize their advertising budget allocation.

Here is a summary of what you will be able to learn in each step by following this quickstart:

Setup Environment: Use stages and tables to ingest and organize raw data from S3 into Snowflake
Data Engineering: Leverage Snowpark for Python DataFrames to perform data transformations such as group by, aggregate, pivot, and join to prep the data for downstream applications
Data Pipelines: Use Snowflake Tasks to turn your data pipeline code into operational pipelines with integrated monitoring
Machine Learning: Process data and run ML Training in Snowflake using Snowpark ML, and register ML model and use it for inference from Snowpark ML Model Registry (currently in public preview)
Streamlit: Build an interactive Streamlit application using Python (no web development experience required) to help visualize the ROI of different advertising spend budgets
In case you are new to some of the technologies mentioned above, here's a quick summary with links to documentation.

What is Snowpark?
Snowpark is the set of libraries and runtimes that securely enable developers to deploy and process Python code in Snowflake.

Client Side Libraries - Snowpark libraries can be installed and downloaded from any client-side notebook or IDE and are used for code development and deployment. Libraries include the Snowpark API for data pipelines and apps and the Snowpark ML API for end to end machine learning.

Elastic Compute Runtimes - Snowpark provides elastic compute runtimes for secure execution of your code in Snowflake. Runtimes include Python, Java, and Scala in virtual warehouses with CPU compute or Snowpark Container Services (public preview) to execute any language of choice with CPU or GPU compute.

Learn more about Snowpark.

What is Snowpark ML?
Snowpark ML includes the Python library and underlying infrastructure for end-to-end ML workflows in Snowflake. With Snowpark ML, data scientists and ML engineers can use familiar Python frameworks for preprocessing, feature engineering, and training models that can be managed entirely in Snowflake without any data movement, silos or governance trade-offs. Snowpark ML has 2 components: Snowpark ML Modeling for model development and Snowpark ML Operations including the Snowpark Model Registry (public preview) for model management and batch inference.

Snowpark

This quickstart will focus on

Snowpark ML Modeling API, which enables the use of popular Python ML frameworks, such as scikit-learn and XGBoost, for feature engineering and model training without the need to move data out of Snowflake.
Snowpark Model Registry, which provides scalable and secure model management of ML models in Snowflake, regardless of origin. Using these features, you can build and operationalize a complete ML workflow, taking advantage of Snowflake's scale and security features.
Feature Engineering and Preprocessing - Improve performance and scalability with distributed execution for common scikit-learn preprocessing functions.

Model Training - Accelerate model training for scikit-learn, XGBoost and LightGBM models without the need to manually create stored procedures or user-defined functions (UDFs), and leverage distributed hyperparameter optimization (public preview).

Snowpark

Model Management and Batch Inference - Manage several types of ML models created both within and outside Snowflake and execute batch inference.

Snowpark

What is Streamlit?
Streamlit enables data scientists and Python developers to combine Streamlit's component-rich, open-source Python library with the scale, performance, and security of the Snowflake platform.

Learn more about Streamlit.

What You Will Learn
How to analyze data and perform data engineering tasks using Snowpark DataFrames and APIs
How to use open-source Python libraries from curated Snowflake Anaconda channel
How to create Snowflake Tasks to automate data pipelines
How to train ML model using Snowpark ML in Snowflake
How to register ML model and use it for inference from Snowpark ML Model Registry (currently in public preview)
How to create Streamlit application that uses the ML Model for inference based on user input
Prerequisites
Git installed
Python 3.11 installed
Note that you will be creating a Python environment with 3.11 in the Get Started step
A Snowflake account with Anaconda Packages enabled by ORGADMIN. If you do not have a Snowflake account, you can register for a free trial account.
A Snowflake account login with ACCOUNTADMIN role. If you have this role in your environment, you may choose to use it. If not, you will need to 1) Register for a free trial, 2) Use a different role that has the ability to create database, schema, tables, stages, tasks, user-defined functions, and stored procedures OR 3) Use an existing database and schema in which you are able to create the mentioned objects.
