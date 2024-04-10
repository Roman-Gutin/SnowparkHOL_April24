
There are two main prerequisites for getting started with Snowpark.
Using Third-Party Packages from Anaconda

Before you start using the packages provided by Anaconda inside Snowflake, you must acknowledge the External Offerings Terms.
Note
You must be the organization administrator (use the ORGADMIN role) to accept the terms. You only need to accept the terms once for your Snowflake account. See Enabling the ORGADMIN role in an account.
Sign in to Snowsight.
Select Admin » Billing & Terms.
In the Anaconda section, select Enable.
In the Anaconda Packages dialog, click the link to review the External Offerings Terms page.
If you agree to the terms, select Acknowledge & Continue.
If you see an error when attempting to accept the terms of service, your user profile might be missing a first name, last name, or email address. If you have an administrator role, refer to Add user details to your user profile to update your profile using Snowsight. Otherwise, contact an administrator to update your account.

Setting Up Your Development Environment for Snowpark Python

Set up your preferred local development environment to build client applications with Snowpark Python.
Prerequisites
The supported versions of Python are 3.8 through 3.11
You can create a Python virtual environment for a particular Python version using tools like Anaconda, Miniconda, or virtualenv.

Step 1:
conda create --name snowpark-de-ml -c https://repo.anaconda.com/pkgs/snowflake python=3.11
Step 2: Activate conda environment snowpark-de-ml by running the following command in the same terminal window
conda activate snowpark-de-ml
Step 3: Install Snowpark Python, Snowpark ML, and other libraries in conda environment snowpark-de-ml from Snowflake Anaconda channel by running the following command in the same terminal window
conda install -c https://repo.anaconda.com/pkgs/snowflake snowflake-snowpark-python snowflake-ml-python pandas notebook
pip install snowflake


Installation should take around 5 minutes. 




Special credits go to the creator of this quickstart -> https://quickstarts.snowflake.com/guide/getting_started_with_dataengineering_ml_using_snowpark_python/#1
