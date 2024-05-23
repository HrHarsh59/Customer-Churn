# Customer Churn Analysis and Prediction

## Project Overview

This project involves analyzing the customer churn dataset from a telecom company named “Neo.” The goal is to identify the factors contributing to customer churn and develop predictive models to identify customers who are likely to churn. By understanding these factors, the company can take proactive measures to retain customers and reduce churn.

## Dataset

The dataset contains information about the telecom company's customers, including their demographics, account information, and usage patterns. For more details about this dataset, you can refer to the data dictionary provided with the dataset.

## Problem Statement

As a data scientist at "Neo," you are tasked with analyzing the customer churn data to find insights and predict churn. The specific tasks include:

1. **Data Manipulation:**
   - Extract specific columns and subsets of data based on various conditions.
   - Perform aggregations and count operations.

2. **Data Visualization:**
   - Create bar plots, histograms, scatter plots, and box plots to visualize different aspects of the data.

3. **Predictive Modeling:**
   - Build and evaluate machine learning models (linear regression, logistic regression, decision tree, random forest) to predict customer churn.

## Tasks To Be Performed

### 1. Data Manipulation

- Extract the 5th column and store it in `customer_5`.
- Extract the 15th column and store it in `customer_15`.
- Extract all the male senior citizens whose payment method is electronic check and store the result in `senior_male_electronic`.
- Extract all customers whose tenure is greater than 70 months or whose monthly charges are more than $100 and store the result in `customer_total_tenure`.
- Extract all customers with a two-year contract, payment method as mailed check, and churn value as 'Yes' and store the result in `two_mail_yes`.
- Extract 333 random records from the customer churn dataframe and store the result in `customer_333`.
- Get the count of different levels from the 'Churn' column.

### 2. Data Visualization

- Build a bar plot for the `InternetService` column:
  - Set x-axis label to ‘Categories of Internet Service’
  - Set y-axis label to ‘Count of Categories’
  - Set the title of the plot to ‘Distribution of Internet Service’
  - Set the color of the bars to ‘orange’

- Build a histogram for the `tenure` column:
  - Set the number of bins to be 30
  - Set the color of the bins to ‘green’
  - Assign the title ‘Distribution of Tenure’

- Build a scatter plot between `MonthlyCharges` and `tenure`:
  - Map `MonthlyCharges` to the y-axis and `tenure` to the x-axis
  - Assign the points a color of ‘brown’
  - Set the x-axis label to ‘Tenure of Customer’
  - Set the y-axis label to ‘Monthly Charges of Customer’
  - Set the title to ‘Tenure vs Monthly Charges’

- Build a box plot between `tenure` and `Contract`:
  - Map `tenure` on the y-axis and `Contract` on the x-axis

### 3. Linear Regression

- Build a simple linear regression model where the dependent variable is `MonthlyCharges` and the independent variable is `tenure`:
  - Divide the dataset into train and test sets in a 70:30 ratio
  - Build the model on the train set and predict the values on the test set
  - Calculate and store the root mean square error

### 4. Logistic Regression

- Build a simple logistic regression model where the dependent variable is `Churn` and the independent variable is `MonthlyCharges`:
  - Divide the dataset in a 65:35 ratio
  - Build the model on the train set and predict the values on the test set
  - Build the confusion matrix and calculate the accuracy score

- Build a multiple logistic regression model where the dependent variable is `Churn` and the independent variables are `tenure` and `MonthlyCharges`:
  - Divide the dataset in an 80:20 ratio
  - Build the model on the train set and predict the values on the test set
  - Build the confusion matrix and calculate the accuracy score

### 5. Decision Tree

- Build a decision tree model where the dependent variable is `Churn` and the independent variable is `tenure`:
  - Divide the dataset in an 80:20 ratio
  - Build the model on the train set and predict the values on the test set
  - Build the confusion matrix and calculate the accuracy

### 6. Random Forest

- Build a Random Forest model where the dependent variable is `Churn` and the independent variables are `tenure` and `MonthlyCharges`:
  - Divide the dataset in a 70:30 ratio
  - Build the model on the train set and predict the values on the test set
  - Build the confusion matrix and calculate the accuracy

## Project Structure

- `Customer_churn_project_assignment.ipynb`: Jupyter Notebook containing the complete analysis, including data manipulation, EDA, and machine learning models.
- `data/customer_churn-1.csv`: Folder containing the dataset used for analysis.
- `README.md`: Project overview and documentation (this file).

## Usage

To run the analysis, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/HrHarsh59/customer-churn-analysis.git
   cd customer-churn-analysis
