# Titanic EDA Notebook

This repository contains a Jupyter Notebook that performs Exploratory Data Analysis (EDA) on the Titanic dataset. The notebook includes steps for data loading, cleaning, visualization, and interpretation, making it suitable for a Data Analyst internship project.

## Repository Contents

- **EDA_Titanic.ipynb**: The Jupyter Notebook with all the code for data preprocessing, exploratory visualizations, and analysis.
- **train.csv**: The Titanic dataset used in the analysis.
- **EDA_Titanic_Report.pdf** (optional): A comprehensive PDF report generated from the analysis.
- **README.md**: This file, providing an overview and instructions for the project.

## Project Overview

The notebook performs the following steps:
1. **Data Loading and Preprocessing**
   - Loads the Titanic dataset using `pandas.read_csv()`.
   - Checks data structure with `.info()` and `.describe()`.
   - Handles missing values by imputing the `Age` using the median, filling `Embarked` with the mode, and dropping the `Cabin` column due to excessive missing values.
2. **Exploratory Data Analysis (EDA)**
   - **Visualizations:**
     - **Countplots** to examine the distribution of survivors and compare genders.
     - **Histograms and Boxplots** to understand the distribution of features such as `Age`, `Fare`, and their relationship with survival.
     - **Scatterplots** to explore relationships between numerical variables.
     - **Pairplots** for multivariate comparisons.
     - **Heatmaps** for correlation analysis.
   - **Observations:**  
     Each plot is accompanied by interpretations highlighting key insights, such as the influence of socio-economic factors on survival or the distribution of ages among survivors.
3. **Report Generation (Optional)**
   - A PDF report can be generated using the FPDF library directly from the notebook code.

## Getting Started

### Prerequisites

- **Python 3.x**
- **Jupyter Notebook**
- Required Python libraries:
  - `pandas`
  - `seaborn`
  - `matplotlib`
  - `fpdf` (only required if you intend to generate the PDF report)

Install the libraries using pip (if not installed):

```bash
pip install pandas seaborn matplotlib fpdf
