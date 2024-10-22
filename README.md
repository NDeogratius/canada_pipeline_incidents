# canada_pipeline_incidents
# Project Title: Visualizing and Classifying Pipeline Incidents in Canada (2008 – 2024)

## Dataset: Pipeline Incident Data (2008 - Present)  
**Dataset Source**: [Canada Energy Regulator](https://open.canada.ca/data/en/dataset/7dffedc4-23fa-440c-a36d-adf5a6cc09f1)

---
## Notebooks
* 5yrForecast: Contains the forecasting model
* pipeline_incidents_etl: Contains the data preprocessing steps
* pipeline_incidents_ml: Contains the machine learning model

---

## 1. Introduction

Pipeline incidents present significant risks to both the environment and public safety. Understanding the root causes and classifying these incidents will aid in predicting potential future incidents, contributing to improved safety standards and damage prevention. Leveraging machine learning (ML) and data visualization techniques can provide actionable insights into incident causes, types, and trends.

This project aims to develop a comprehensive data analysis and machine learning pipeline to classify and visualize pipeline incidents. The dataset contains detailed information on pipeline incidents from 2008 to the present, with over 1,800 rows and 102 columns, including data on incident types, geographic locations, companies involved, and volume released.

---

## 2. Objectives

The primary objectives of this project are to:

1. **Classify Incidents**: Train machine learning models to classify incident emergency levels, based on relevant features like location, equipment, and companies involved.
2. **Analyze Incident Patterns**: Identify trends in pipeline incidents, including temporal, geographic, and equipment-related patterns.
3. **Visualize Data and Predictions**: Develop interactive visualizations and dashboards using Tableau and Plotly to allow users to explore incidents dynamically.
4. **Provide Advanced Reporting**: Use Tableau for interactive dashboards and advanced data visualization to present findings in a user-friendly way for stakeholders.

---

## 3. Data Overview

**Dataset**: The dataset contains 1,892 rows and 102 columns of various data types. Key columns include:

- **Incident Number**: Unique identifier for each incident.
- **Incident Types**: Classifications such as fire, release of substances, or adverse environmental effects.
- **Reported Date**: Date of the incident report.
- **Emergency Level**: The level of emergency (on a scale of 1 to 3, with 3 being the most severe or hazardous) based on the level of severity and potential hazards to the public and environment.
- **Nearest Populated Centre**: The nearest populated location and province where the incident occurred.
- **Company**: The company involved in the incident.
- **Latitude/Longitude**: Geographical coordinates of the incidents.
- **Volume Released**: Volume of substances released during the incidents.
- **Equipment and Maintenance**: Details about equipment failure, inspections, and maintenance work.

---

## 4. Project Workflow

### 4.1 Data Preprocessing (Pandas)
- **Data Cleaning**: Load the dataset and clean missing or inconsistent data.
- **Handling Missing Values**: Address missing data by using imputation techniques or removing rows where appropriate.
- **Encoding Categorical Data**: Convert categorical variables (e.g., Company, Province) into numerical formats using methods like one-hot encoding.
- **Feature Selection**: Select relevant features such as equipment type, geographic location, maintenance details, and incident type for analysis.

### 4.2 Data Analysis and Visualization (Matplotlib, Plotly)
- **Incident Trends**: Generate time-series plots and bar charts to visualize incident frequencies by year, month, and company.
- **Geographical Patterns**: Use latitude and longitude data to create heatmaps or scatter plots showing incident locations and volumes released.
- **Proximity Analysis**: Analyze incident locations relative to populated centers and visualize incident "hotspots."

### 4.3 Machine Learning Model Training (Scikit-learn)
- **Classification Models**: Train ML algorithms such as Logistic Regression, Random Forest, and Decision Trees to classify incidents based on other features in the dataset.
- **Model Evaluation**: Evaluate model performance using metrics such as accuracy, precision, recall, and F1 score.
- **Hyperparameter Tuning**: Use techniques such as grid search to optimize model performance.

### 4.4 Advanced Reporting and Visualization (Tableau)
- **Interactive Dashboard**: Develop a Tableau dashboard with filters to allow users to explore incidents by company, location, date, and incident type.
- **Integration with ML Predictions**: Integrate machine learning predictions into the Tableau dashboard for an end-to-end solution.
- **Geographical Visualization**: Use Tableau's mapping capabilities to display the locations of pipeline incidents and their characteristics.

---

## 5. Tools and Technologies

1. **Pandas**: For data preprocessing, cleaning, and manipulation.
2. **Scikit-learn**: For training and evaluating machine learning models.
3. **Matplotlib and Plotly**: For creating static and interactive visualizations.
4. **Tableau**: For creating interactive dashboards and advanced visualizations.

---

## 6. Use Cases

1. **Incident Classification**: Predict the type of incident (e.g., fire, environmental effect) based on features like equipment type and geographical data.
2. **Incident Hotspot Visualization**: Identify geographic locations that experience a high number of incidents and visualize these as heatmaps.
3. **Company-Specific Insights**: Allow users to explore incident data for specific companies and compare their safety records.
4. **Predictive Maintenance**: Predict potential equipment failure or maintenance needs based on historical data.

---

## 7. Expected Outcomes

- A robust machine learning model that accurately classifies pipeline incidents.
- An interactive Tableau dashboard for easy exploration and reporting.
- Insights into the most common incident types, affected areas, and trends over time.

---

## 9. Conclusion

By integrating machine learning, data analysis, and interactive visualizations, this project will provide an effective tool for understanding and predicting pipeline incidents. The insights generated from this analysis can be invaluable to regulators, companies, and policymakers in improving pipeline safety across Canada.

