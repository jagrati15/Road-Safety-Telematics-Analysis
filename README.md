# Road Safety Telematics Analysis 🚗

## Overview
This capstone project, developed at CU Boulder, explores how telematics data (GPS, speed, acceleration, etc.) can be used to profile driver behavior and enhance road safety. We applied clustering and classification techniques to identify risky drivers and suggest targeted policy actions.

## Objectives
- Perform EDA on raw telematics data from drivers
- Identify risky driving behavior using unsupervised learning (KMeans, DBSCAN)
- Classify driver profiles based on safety metrics
- Provide actionable insights for insurance providers and road safety experts

## Dataset
The dataset consisted of time-series vehicle telematics data including GPS coordinates, speed, acceleration, and more, recorded over multiple driving sessions.

## Tools & Technologies
- Python: pandas, numpy, matplotlib, seaborn
- Machine Learning: scikit-learn (KMeans, Logistic Regression, DBSCAN)
- Clustering and classification algorithms
- Jupyter Notebooks, Google Colab
- GitHub

## Results and Findings

- Successfully extracted over **6,193 trips** from 157 drivers using telematics and V2X sensor data.
- Built driver profiles based on:
  - Sudden acceleration/deceleration events
  - Speeding behavior vs speed limits
  - Yaw rate analysis for turns and lane changes
- Developed a **penalty scoring system** using multi-threshold percentiles (99th, 97.5th, 95th) to rank aggressive behavior.
- Integrated **OpenStreetMap** speed limits and imputed ~30% of missing values using regression models.
- Applied **KMeans clustering** to group drivers into 3 behavioral segments:
  1. Law-abiding and cautious
  2. Consistently slow drivers
  3. Speeding and aggressive drivers
- Achieved strong data enrichment and behavioral segmentation through a mix of EDA, clustering, and hypothesis testing.


## Folder Structure
```
. ├── data/ # Raw and processed datasets
├── notebooks/ # Jupyter Notebooks for EDA, clustering, feature engineering
├── visuals/ # Plots and visualizations used in analysis & README
├── README.md # Project summary and insights
├── LICENSE # MIT License
└── requirements.txt # Python dependencies
```

## Medium Article
📄 [Read the Full Write-up](https://medium.com/99p-labs/enhancing-road-safety-telematics-data-analysis-and-driver-profiling-cu-boulder-capstone-b72129e14325)

