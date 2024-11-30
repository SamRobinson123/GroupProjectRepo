# Swire Coca-Cola Capstone Modeling

This portfolio highlights the **Swire Coca-Cola Capstone Project**, which focuses on predicting machine failure to reduce downtime and improve operational efficiency. A key component of the project is the development of **Survival Models** to estimate the time to failure for machines. Click the links below to view the code and presentation slides on my personal GitHub page.

## [Group6Capstone: Project Overview](https://github.com/SamRobinson123/GroupProjectRepo/blob/main/Group6Capstone.ipynb)
## [Group6 Slide Deck: Presentation Slides](https://github.com/SamRobinson123/GroupProjectRepo/blob/main/Group6SlideDeck.pdf)
![Project Status](https://img.shields.io/badge/status-complete-green.svg)

### Business Problem
Swire Coca-Cola incurs an annual loss of approximately **$60 million** due to unplanned machine downtimes. Current maintenance practices are reactive, causing delays in repairs and reduced productivity. The goal of this project is to build predictive models to forecast machine failure and enable proactive maintenance. This approach aims to minimize downtime, optimize maintenance schedules, and improve overall efficiency.

### 🎯 Objective
The primary focus of this project is to:
- Develop **Survival Analysis Models** to predict the time to failure for machines and their components.
- Utilize these predictions to transition from reactive to proactive maintenance workflows.
- Reduce operational losses caused by downtime and improve machine uptime.

### 📊 Project Details
- **Dataset**: The project utilized machine maintenance data, including `FUNCTIONAL_LOC` (machine IDs) and `EQUIPMENT_ID` (component IDs), with event times for unplanned maintenance.
- **Data Cleaning**:
  - Filtered down to data with sufficient completeness and consistency.
  - Addressed missing values and removed entries with unreliable machine start dates.
- **Modeling**:
  - Developed two **Kaplan-Meier Survival Models**:
    1. **Machine-Level Survival Model**: Focused on predicting the lifespan of individual machines (`FUNCTIONAL_LOC`).
    2. **Component-Level Survival Model**: Focused on predicting the time to failure of specific components within machines (`EQUIPMENT_ID`).
  - Both models achieved **Concordance Index (C-Index)** scores of:
    - **Machine-Level Model**: 0.78
    - **Component-Level Model**: 0.76

### 🚀 Value of the Solution
The survival models provide valuable insights for Swire Coca-Cola by:
- Enabling **proactive maintenance** to prevent machine downtime.
- Improving decision-making with data-driven predictions.
- Laying the groundwork for further improvements through enhanced data collection and feature engineering.

### Key Metrics
- **Concordance Index (C-Index)**:
  - **Machine-Level Survival Model**: 0.78
  - **Component-Level Survival Model**: 0.76
- These metrics indicate that the survival models are effective at predicting machine and component lifespans, even with limited data.

---

### Takeaways
Key insights from this project include:
- **Survival Analysis** is a promising approach for predicting time to failure in manufacturing systems.
- Improved data quality and additional features (e.g., machine age, temperature, pressure) could significantly enhance model performance.
- Filtering the dataset for reliable entries ensured the survival models could produce meaningful predictions.

---
