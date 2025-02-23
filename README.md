# DataNear-Earth Object (NEO) Hazard Prediction
This project aims to analyze and predict Near-Earth Objects (NEOs) that may pose a threat to Earth. Using NASA's dataset from 1910 to 2024, we apply data analysis, preprocessing, and machine learning techniques to classify whether an object is hazardous or not.-Science

Dataset
The dataset consists of 338,199 records representing space objects tracked for their proximity to Earth.
It includes the following key features:

absolute_magnitude: 
The object's absolute brightness.
estimated_diameter_min/max:
Estimated minimum and maximum diameter (in km).
orbiting_body: 
The celestial body the object orbits (e.g., Earth).
relative_velocity: 
The object's velocity relative to Earth (in km/h).
miss_distance: 
The closest distance between the object and Earth (in km).
is_hazardous: 
The target variable (True if the object is hazardous, False otherwise).



Data Processing and Analysis
 1. Data Cleaning
Checked for missing values and filled them using the mean for numerical columns.
Encoded categorical variables (orbiting_body) using Label Encoding.
 2. Exploratory Data Analysis (EDA)
Plotted distribution of hazardous vs non-hazardous NEOs.
Visualized feature distributions (absolute magnitude, diameters, velocities, etc.).
Used Heatmap (correlation matrix) to analyze relationships between features.
 3. Data Preprocessing
Selected key features for training.
Applied StandardScaler to normalize numerical features.
Split the dataset into 80% training and 20% testing.



Machine Learning Model
 Logistic Regression Model
Used class_weight="balanced" to handle imbalanced data.
Achieved AUC-ROC Score = 0.80, with:
Recall = 88% for hazardous objects (good detection rate).
Precision = 31% (needs improvement).
