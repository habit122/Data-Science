🌍 Near-Earth Object (NEO) Hazard Prediction

📌 Project Overview

This project analyzes and predicts Near-Earth Objects (NEOs) that could pose a threat to Earth. Using NASA's dataset (1910 - 2024), we employ data science, exploratory analysis, and machine learning to classify whether an object is hazardous.

🚀 Key Objectives:

📊 Analyze NEO data to identify key trends.

🔍 Perform Exploratory Data Analysis (EDA) to detect patterns.

🤖 Train a machine learning model to predict hazardous asteroids.

🎯 Optimize performance for better prediction accuracy.

📂 Dataset Description

Dataset Source: NASA NEO Dataset

Feature

Description

absolute_magnitude

The object's absolute brightness.

estimated_diameter_min/max

Estimated diameter range (km).

orbiting_body

The celestial body the object orbits (e.g., Earth).

relative_velocity

The object's speed relative to Earth (km/h).

miss_distance

The closest distance between the object and Earth (km).

is_hazardous

Target variable (1 = Hazardous, 0 = Non-Hazardous).

📊 Exploratory Data Analysis (EDA)

✅ Key Analysis Performed:

Distribution Analysis 📊

Visualized the distribution of hazardous vs. non-hazardous NEOs.

Checked the distribution of diameters, velocities, and distances.

Feature Correlation (Heatmap) 🔥

Identified relationships between features using correlation matrix.

Observed strong correlation between diameter features.

Outlier Detection 🚀

Checked for extreme values in velocity and distance features.

Analyzed if outliers impact model performance.

🤖 Machine Learning Model

✅ Logistic Regression Model

Handled class imbalance using class_weight='balanced'.

Performance Metrics:

📈 ROC-AUC Score: 0.80

🎯 Recall for hazardous objects: 88% (high detection rate)

⚠️ Precision: 31% (some false positives)



🔍 Key Findings and Insights

Most NEOs are non-hazardous, with only a small percentage classified as potentially dangerous.

Larger asteroids (higher diameter values) tend to have a higher likelihood of being hazardous, though not all large objects pose a risk.

Relative velocity and miss distance do not strongly correlate with hazard classification, indicating that other features may play a bigger role in determining risk.

The model performs well in detecting hazardous objects (high recall), but suffers from low precision, meaning some non-hazardous objects are misclassified as dangerous.

Feature selection and engineering improvements could enhance the predictive power of the model, particularly by considering additional astronomical data.


