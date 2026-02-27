# Exploratory and Predictive Analysis of Industrial Machine Failures

**Author:** Gamze Esen Erdemir

## 1. Introduction & Overview

In modern industry, the reliability of machinery plays a critical role in ensuring smooth operations, reducing unexpected downtime, and optimizing productivity and profit. Predicting equipment failure—commonly known as **predictive maintenance**—allows organizations to address issues proactively, saving both time and costs while improving worker safety.

This project focuses on analyzing real-world manufacturing sensor data to build a **predictive model** that classifies whether a machine will fail based on various operational and environmental conditions, such as temperature, rotational speed, torque, and tool wear.

### Primary Goals
- **Identify Factors:** Discover which factors most strongly correlate with machinery failure.
- **Model Failure Risk:** Demonstrate how a simple machine learning model (Logistic Regression) can classify failure risk based on sensor data.
- **Foundation for Smart Monitoring:** Provide a basis for building smart monitoring systems in industrial environments.

## 2. Methodology & Dataset

The analysis utilizes the [AI4I 2020 Predictive Maintenance Dataset](https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset) from the UCI Machine Learning Repository. 

The dataset contains 10,000 observations and 14 features, including:
- **Product ID / Type:** Quality variants (L, M, H).
- **Temperatures [K]:** Air and process temperatures.
- **Rotational speed [rpm] & Torque [Nm]:** Machine operational parameters.
- **Tool wear [min]:** Running wear time of the tool.

### Failure Modes Overview
The overarching `Machine failure` label is set to 1 if the machine fails due to any of five independent failure modes:
1. Tool wear failure (TWF)
2. Heat dissipation failure (HDF)
3. Power failure (PWF)
4. Overstrain failure (OSF)
5. Random failures (RNF)

## 3. Workflow

The analytical workflow encompasses:
1. **Exploratory Data Analysis (EDA):** To uncover and visualize relationships between operational parameters and failure events.
2. **Data Preprocessing:** Cleaning and preparing the dataset for model training.
3. **Model Building:** Constructing a **Logistic Regression** classifier to predict failure occurrences.
4. **Evaluation:** Utilizing standard classification metrics (such as the confusion matrix and classification report) to determine model accuracy and robustness.

---

### Acknowledgement
- **Data Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/) for providing the dataset.
- **Guidance:** Dr. Steven Livingstone for course materials and lectures guiding this methodology.
