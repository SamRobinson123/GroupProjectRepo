# Swire Coca-Cola Capstone Modeling

This portfolio showcases the Data Science Capstone project undertaken by Group 6. The project focuses on reducing operational inefficiencies at Swire Coca-Cola through predictive modeling techniques. Click the link below to view the code on my personal GitHub page.

## [Group6Capstone: Project Overview](https://github.com/SamRobinson123/GroupProjectRepo/blob/main/Group6Capstone.ipynb)
![Project Status](https://img.shields.io/badge/status-complete-green.svg)

### Business Problem
Swire Coca-Cola incurs an annual loss of approximately **$60 million** due to machine downtimes. Currently, maintenance workers respond reactively to machine breakdowns, leading to prolonged downtimes and productivity losses. This project aims to develop a **predictive model** that alerts workers of machines with a high probability of malfunction before the incidents occur. The solution seeks to minimize downtime, improve operational efficiency, and drive significant cost savings for Swire Coca-Cola.

### 🎯 Objective
The primary goal of this project is to:
- Build a **predictive model** to forecast machine failures and time to failure.
- Enable proactive maintenance scheduling to reduce machine downtime.
- Enhance productivity and reduce costs by improving machine uptime.

### 📊 Project Details
- **Dataset**: The project utilizes a dataset containing operational metrics from Swire Coca-Cola's manufacturing machines.
- **Data Cleaning**:
  - Handled missing values and inconsistent data points.
  - Transformed variables to align with the target outcome (time to failure).
  - Selected features relevant to machine malfunction predictions.
- **Modeling**:
  - Implemented a **Random Forest Regressor** and **XGBoost** for predictive modeling.
  - Conducted hyperparameter tuning using GridSearchCV for optimal performance.
  - Evaluated models using metrics such as Mean Squared Error (MSE) and R-squared.

### 🚀 Value of the Solution
This project delivers significant value to Swire Coca-Cola by:
- Reducing annual losses attributed to machine downtimes.
- Transitioning from reactive to proactive maintenance workflows.
- Enabling data-driven decision-making in maintenance operations.

### Key Metrics
- **Mean Squared Error (MSE)**: [Insert Value]
- **R-Squared**: [Insert Value]

These metrics highlight the model's strong predictive capability and its potential for real-world application.

### Takeaways
Key learnings from this project include:
- The importance of thorough **data cleaning** and **preparation** in predictive modeling.
- The efficacy of using ensemble models like Random Forest and XGBoost for complex regression tasks.
- The value of hyperparameter tuning in optimizing model performance.

### 📈 Exploratory Data Analysis (EDA) Examples
The following visualization was critical during the data exploration phase and provides insights into machine downtimes:

#### Example Graph: Distribution of Machine Downtimes
![Sample Graph](sample_graph.png)

This graph illustrates downtime patterns and helps identify high-risk periods for machine failures. Additional visualizations and analyses can be found in the full notebook.

---

## Setup and Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/SamRobinson123/GroupProjectRepo.git
   cd GroupProjectRepo
