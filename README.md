# Project Overview


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
ª   blogpost.txt - content used on the blog post hosted on Medium
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
 - A databricks cluster running 11.3

```
poetry install
```
__note__: It is possible to run the code without poetry and running it elsewhere (locally / on other cloud providers, although some code re-factoring will be required.)