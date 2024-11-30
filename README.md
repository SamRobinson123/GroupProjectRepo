from nbformat import read

# Define the file path to your notebook
file_path = r'C:\Users\sarob\OneDrive - TRICENTIS\Documents\Git Hub\GroupProjectRepo\Group6Capstone.ipynb'

# Load the Jupyter Notebook file
with open(file_path, 'r', encoding='utf-8') as file:
    notebook = read(file, as_version=4)

# Extract details such as notebook metadata and a summary of its contents
notebook_cells = notebook['cells']
notebook_metadata = notebook.get('metadata', {})

# Summarize the contents
notebook_content_summary = {
    "total_cells": len(notebook_cells),
    "code_cells": len([cell for cell in notebook_cells if cell['cell_type'] == 'code']),
    "markdown_cells": len([cell for cell in notebook_cells if cell['cell_type'] == 'markdown']),
    "raw_cells": len([cell for cell in notebook_cells if cell['cell_type'] == 'raw'])
}

# Generate a README file template
readme_content = f"""
# Group6Capstone Project

This repository contains the Jupyter Notebook file **`Group6Capstone.ipynb`**, which is the primary deliverable for the Group 6 Capstone Project. This README provides an overview of the notebook's contents, its objectives, and how to run the analyses contained within.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Notebook Contents](#notebook-contents)
3. [Setup and Installation](#setup-and-installation)
4. [Usage](#usage)
5. [Outputs](#outputs)
6. [Contributing](#contributing)
7. [License](#license)

---

## Project Overview

The Group6Capstone project aims to address [briefly describe the project's objective, e.g., analyze data, build a predictive model, etc.]. The notebook includes data preprocessing, exploratory data analysis (EDA), modeling, and visualizations to support the project's goals.

---

## Notebook Contents

The **`Group6Capstone.ipynb`** notebook consists of the following sections:

- **Introduction and Objective**: Explains the purpose of the project and its scope.
- **Data Loading and Preprocessing**: Steps to import and clean the dataset(s) used.
- **Exploratory Data Analysis (EDA)**: Key insights from visualizations and summary statistics.
- **Feature Engineering**: Details the process of creating and selecting features for modeling.
- **Model Development**: Includes the models built, their hyperparameter tuning, and evaluation metrics.
- **Results and Discussion**: Highlights key findings and their implications.
- **Conclusion and Future Work**: Summarizes the project and suggests next steps.

### Summary Statistics

- **Total Cells**: {notebook_content_summary['total_cells']}
- **Code Cells**: {notebook_content_summary['code_cells']}
- **Markdown Cells**: {notebook_content_summary['markdown_cells']}
- **Raw Cells**: {notebook_content_summary['raw_cells']}

---

## Setup and Installation

To run this notebook locally, ensure the following are installed:

1. **Python 3.8 or higher**
2. Required Python libraries (listed in `requirements.txt`):

```bash
pip install -r requirements.txt
