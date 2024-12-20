# Telecom Churn Dataset Project

This repository contains a detailed end-to-end analysis of a telecom churn dataset. The project includes steps for data preprocessing, exploratory data analysis (EDA), feature engineering, and visualization using bar charts, pie charts, and statistical summaries.

## Project Overview

This project demonstrates the following key steps:

1. **Data Loading**: Import and examine the dataset.
2. **Data Preprocessing**: Handle missing values, incorrect data types, and outliers.
3. **Exploratory Data Analysis (EDA)**:
   - Analyze categorical and numerical columns.
   - Create frequency tables, bar charts, pie charts, and histograms.
4. **Feature Engineering**: Encode categorical variables and scale numerical variables.
5. **Correlation Analysis**: Visualize relationships between numerical features using a heatmap.
6. **Outlier Treatment**: Use interquartile range (IQR) for outlier detection and imputation.
7. **Visualization**: Generate meaningful insights through visualizations.

## Repository Structure

```
.
├── Churn_data_set_project_.ipynb       # Main Jupyter Notebook
├── README.md                           # Project Documentation
├── processed_data.csv                  # Processed dataset (example output)
```

## Key Features

### Data Preprocessing
- **Handling Missing Values**:
  - Categorical columns: Filled with the mode.
  - Numerical columns: Imputed using KNNImputer.
- **Data Cleaning**:
  - Dropped irrelevant columns (`year`, `customer_id`, `phone_no`).
  - Fixed corrupted entries (e.g., numerical values in categorical columns).

### Exploratory Data Analysis (EDA)

#### Categorical Features:
- Created frequency tables.
- Generated **bar charts** and **pie charts** for visualizing value distributions.

#### Numerical Features:
- Plotted histograms, distribution plots, and box plots to study data distributions.
- Used IQR for outlier detection and imputation.

#### Correlation Analysis:
- Displayed relationships between numerical features using a heatmap.

### Feature Engineering
- Encoded categorical columns using LabelEncoder.
- Scaled numerical data using standardization (Z-score normalization) and Min-Max normalization.

## Sample Visualization

### Bar Chart Example:

```python
import matplotlib.pyplot as plt
import seaborn as sns

plt.figure(figsize=(12, 4))
for idx, column in enumerate(cat, 1):
    plt.subplot(1, len(cat), idx)
    sns.countplot(data=tele, x=column)
    plt.title(column)
plt.tight_layout()
plt.show()
```

### Output:
![Bar Chart](example_bar_chart.png)  

## Prerequisites

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   ```
2. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Churn_data_set_project_.ipynb
   ```
3. Run the notebook cells sequentially to replicate the analysis.

## Dataset

The dataset used in this project contains customer attributes and churn-related information. This dataset can be used to build predictive models for churn analysis.

## Author

**Satish Kumar Dwivedi**  
[LinkedIn](https://www.linkedin.com/in/satish-dwivedi-1291b1227)


