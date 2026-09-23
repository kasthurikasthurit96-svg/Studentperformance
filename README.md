# Student Performance Data Understanding, Cleaning & Feature Engineering

## Project Overview

This project focuses on understanding, cleaning, and analyzing student performance data.

The dataset contains student demographic information, parental education, lunch details, test preparation information, and subject-wise scores.

The project performs data cleaning, statistical analysis, feature engineering, and outlier detection.

## Objectives

- Clean categorical features.
- Analyze student subject scores using statistical measures.
- Calculate total marks.
- Calculate percentage performance.
- Detect extreme performance outliers.
- Visualize student performance.
- Categorize students based on their percentage.

## Dataset Features

The dataset contains the following important attributes:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch
- Test Preparation Course
- Math Score
- Reading Score
- Writing Score

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

## Data Cleaning

The following categorical features were cleaned:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch
- Test Preparation Course

Missing categorical values were handled using the mode, and text values were standardized using lowercase and whitespace removal.

## Statistical Analysis

Statistical measures were calculated for:

- Math Score
- Reading Score
- Writing Score

The following measures were analyzed:

- Mean
- Median
- Standard Deviation
- Minimum
- Maximum
- First Quartile (Q1)
- Third Quartile (Q3)

## Feature Engineering

Two new features were created.

### Total Marks

Total marks are calculated by adding the scores of all three subjects.

```text
Total Marks = Math Score + Reading Score + Writing Score
````

### Percentage

Percentage performance is calculated based on the maximum total marks of 300.

```text
Percentage = (Total Marks / 300) × 100
```

## Outlier Detection

The Interquartile Range (IQR) method was used to detect extreme performance values.

```text
IQR = Q3 - Q1

Lower Limit = Q1 - 1.5 × IQR

Upper Limit = Q3 + 1.5 × IQR
```

Outliers were detected separately for:

* Math Score
* Reading Score
* Writing Score

A boxplot was also created to visualize the outliers.

## Performance Categorization

Students were categorized based on their percentage:

* 75% and above – Excellent
* 60% to 74% – Good
* 40% to 59% – Average
* Below 40% – Poor

## Visualizations

The project includes:

* Subject-wise average score chart
* Total marks distribution
* Percentage distribution
* Subject score correlation heatmap
* Subject score boxplot for outlier detection

## Project Workflow

```text
Load Dataset
      ↓
Understand Dataset
      ↓
Clean Categorical Features
      ↓
Check Missing Values
      ↓
Calculate Statistical Measures
      ↓
Create Total Marks
      ↓
Calculate Percentage
      ↓
Detect Outliers
      ↓
Create Visualizations
      ↓
Categorize Student Performance
      ↓
Save Cleaned Dataset
```

## How to Run

1. Open Google Colab.
2. Upload the student performance CSV dataset.
3. Run the cells one by one.
4. Check the statistical results.
5. View the generated graphs.
6. Check the detected outliers.
7. The cleaned dataset will be saved as:

```text
Student_Performance_Cleaned.csv
```

# Plot Overview

<img width="1074" height="683" alt="image" src="https://github.com/user-attachments/assets/3f5f49ee-8a3d-4831-965f-f1d4d80299e9" />

<img width="865" height="595" alt="image" src="https://github.com/user-attachments/assets/1d814313-2dcf-4a1b-87eb-4dfff6d3eda6" />

<img width="878" height="591" alt="image" src="https://github.com/user-attachments/assets/d31b91cc-179c-48bd-880f-53e182bdfab7" />

<img width="809" height="666" alt="image" src="https://github.com/user-attachments/assets/b4018201-936d-4a72-b18d-4c94dfe33d02" />



## Conclusion

This project provides a complete understanding of student performance data through data cleaning, statistical analysis, feature engineering, and outlier detection.

The newly created Total Marks and Percentage features make it easier to analyze overall student performance. Outlier detection helps identify unusually high or low scores across different subjects.

## Author

**Kasthuri T**
