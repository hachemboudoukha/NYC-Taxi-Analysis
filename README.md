
# NYC Taxi Trip Data Analysis


Welcome to my NYC Taxi Trip Data Analysis project! This repository showcases the work I have done as a junior data scientist to analyze and model New York City taxi trip data for January 2025. Below, I explain what I did step by step and summarize the results of my analysis.

---

## **Table of Contents**
0. [Import libraries](#imports)
1. [Import data](#data_import)
2. [Data visualization](#visualization)
3. [Data cleaning](#cleaning)
4. [Data preparation](#preparation)
5. [Benchmark model](#benchmark_model)<br>
    5.1. [Train-test split](#train_test_split)<br>
4. [Data preparation](#model_training)

---

## **What I Did**

### **1. Imported Libraries** <a name="imports"></a>
[Back to top](#table_of_contents)

I started by importing essential Python libraries such as:
- `pandas` for data manipulation
- `numpy` for numerical operations
- `matplotlib` and `seaborn` for data visualization
- `scikit-learn` for machine learning modeling

import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
import seaborn as sns


### **2. Loaded the Dataset** <a name="data_import"></a>
[Back to top](#table_of_contents)

I worked with the NYC Yellow Taxi trip dataset for January 2025, which was provided in `.parquet` format. The dataset contains detailed information about taxi trips, including:
- Pickup and drop-off times
- Trip distances
- Passenger counts
- Fare details (e.g., fare amount, tips, total amount)



### **3. Data Exploration and Visualization** <a name="visualization"></a>
[Back to top](#table_of_contents)

I explored the dataset to understand its structure and identify key patterns:
- Visualized distributions of trip distances, fare amounts, and passenger counts.
- Analyzed trends over time (e.g., hourly, daily patterns).
- Identified outliers such as negative fares or unusually high values.



### **4. Data Cleaning** <a name="cleaning"></a>
[Back to top](#table_of_contents)

To ensure data quality, I performed the following steps:
- Removed rows with missing or invalid values (e.g., negative fares).
- Filtered out extreme outliers that could skew the analysis.
- Ensured consistency in categorical variables like payment types.

#### **5.1. Train-test split** <a name="train_test_split"></a>
[Back to top](#table_of_contents)
- Split the data into training and testing sets to evaluate model performance.



### **6. Built a Benchmark Model** <a name="benchmark_model"></a>
[Back to top](#table_of_contents)

I trained a simple machine learning model to predict taxi fare amounts based on trip distance, time of day, and other features:
- Used a `DecisionTreeRegressor` as the benchmark model.





---

## **Results**

### **Insights from Data Analysis**
1. **Trip Patterns:**
   - Most trips occurred during rush hours (morning and evening).
   - Weekends had fewer trips compared to weekdays.

2. **Fare Trends:**
   - Fare amounts were generally proportional to trip distances.
   - Short trips within Manhattan had higher average fares per mile compared to longer trips.

3. **Impact of Weather:**
   - Rainy days showed a slight increase in trip fares due to longer travel times.

### **Model Performance**
The benchmark model achieved the following results:
- **Mean Absolute Error (MAE):** ~3.50 USD  
  This indicates that the model's predictions were off by an average of $3.50 compared to actual fare amounts.


---

## **How to Use This Project**

1. Clone this repository:

```
git clone https://github.com/your-repo-name/nyc-taxi-analysis.git


cd nyc-taxi-analysis
```

2. Install required dependencies:
```
pip install pandas numpy matplotlib seaborn scikit-learn
```


3. Open the Jupyter Notebook (`notebook_taxi_nyc.ipynb`) to explore the analysis and results step by step.



## **What I Learned**
This project helped me build skills in:
1. Cleaning and preparing real-world datasets.
2. Performing exploratory data analysis (EDA) using visualizations.
3. Building and evaluating machine learning models.
4. Understanding how external factors (e.g., weather) impact predictions.

