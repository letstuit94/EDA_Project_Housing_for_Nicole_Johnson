# EDA Project Housing for Nicole Johnson

This project presents an exploratory data analysis of the King County housing market using Python and SQL. The objective is to identify key factors influencing house prices and derive data-driven recommendations for a specific buyer persona, Nicole Johnson. She is looking to move within the next year into a central, lively neighborhood and is focusing on the mid-range price segment. The analysis aims to uncover optimal property characteristics and support informed decision-making in a competitive real estate market.

The purchase recommendation for Nicole Johnson is developed collaboratively by:
	•	Stuart
	•	Vasyl
	•	Jennifer

Together, the team combines data analysis, statistical modeling, and domain insights to deliver a comprehensive, data-driven housing recommendation.

## Requirements

- pyenv
- python==3.11.3

## Setup

One of the first steps when starting any data science project is to create a virtual environment. For this project you have to create this environment from scratch yourself. However, you should be already familiar with the commands you will need to do so. The general workflow consists of... 

* setting the python version locally to 3.11.3
* creating a virtual environment using the `venv` module
* activating your newly created environment 
* upgrading `pip` (This step is not absolutely necessary, but will save you trouble when installing some packages.)
* installing the required packages via `pip`

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

*Note: We do have the `requirements.txt` in the repository but please try to first install packages by yourself.*

At the end, you want to make sure that people who are interested in your project can create an identical environment on their own computer in order to be able to run your code without running into errors. Therefore you can create a `requirements file` and add it to your repository. You can create such a file by running the following command: 

```bash
pip freeze > requirements.txt
```

*Note: In rare case such a requirements file created with `pip freeze` might not ensure that another (especially M1 chip) user can install and execute it properly. This can happen if libraries need to be compiled (e.g. SciPy). Then it also depends on environment variables and the actual system libraries.*

## Presentation
```bash
pip install RISE

jupyter nbconvert 1_task_preparation_and_descriptive_statistics.ipynb --to slides --no-input --post serve

jupyter nbconvert 2_Exploratory_Data_Analysis.ipynb --to slides --no-input --post serve

jupyter nbconvert 3_Sales_presentation_for_NJ.ipynb --to slides --no-input --post serve
```

if server in use, then switch to a free port: 
```bash
jupyter nbconvert 3_Sales_presentation_for_NJ.ipynb \
  --to slides \
  --no-input \
  --post serve \
  --ServePostProcessor.port=8001
```
--- 
## In Case of Failure
If you fail to do the setup by yourself, then please revisit the previous repositories where you have done the setup and follow those steps.
