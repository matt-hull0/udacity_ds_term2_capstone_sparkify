# Project Overview

A blog post covering the work done on this project can be found here:
https://medium.com/@matthewhull55/predicting-user-churn-using-spark-08f892c55393

This repo covers my work done for the Data Scientist Capstone project as a part of term 2 of the Udacity Data Science Nano Degree program.

I chose to work on the project based around the fictional music streaming service, “Sparkify”, where we are tasked to identify users that are likely to churn. This is a typical task within the data science domain, so that action can be taken to retain (such as offering a discount) the customers. In this case we could choose to look at either users of the paid subscription, or the free service, which still brings in revenue through advertising. I specifically chose this project as spark had not been covered in the Nanodegree up to now, whilst it is used at my place of work so I was keen to improve my knowledge.

Using Spark, running on a databricks cluster on Microsofts Azure services, I was able to analyse the full 12Gb input file provided by Udacity. The data covers interactions users have with the service, such as logging up, up/down grading their accounts, and of course listening to songs.

I performed exploratory analysis on the data, then from those insights cleaned it and generated features which were passed to cross validation pipelines for two different types of models with different hyper-parameters to tune. The best model was found from my selections, the results of which are presented in the notebook in this repository and reviewed in my blog post linked above.

# Libraries Used:
```
python = "~3.9"
ydata-profiling = "^4.3.1"
databricks-connect = "~11.3"
ipykernel = "^6.28.0"
pyarrow = "^14.0.2"
ipywidgets = "^8.1.1"
pandas = "^2.1.4"
matplotlib = "^3.8.2"
seaborn = "~0.12"
```

Refer to the poetry.lock file for the exact versions of all libraries (including sub-dependancies) that were used.

# File Structure:

```bash
ª   .gitignore
ª   blogpost.txt - draft of the content used on the blog post hosted on Medium
ª   notebook.ipynb - Jupyter notebook with all the code and analysis
ª   poetry.lock - file used by Poetry package manager
ª   poetry.toml - file used to specify poetry config
ª   pyproject.toml - file used to specify libraries
ª   README.md
+---blog_post_materials - directory for storing blog post images
```
# To run locally:

Pre-requisites
 -  `poetry` package manager
 - A databricks environment setup connected with databricks-connect
 - A databricks cluster running 11.3 ML

```
poetry install
```
__note__: It is possible to run the code without poetry and running it elsewhere (locally / on other cloud providers, although some code re-factoring will be required.)