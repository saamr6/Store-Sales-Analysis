# Store-Sales-Analysis
Exploratory Data Analysis (EDA) and visualization of store sales data using Python, Pandas, and Matplotlib. This notebook includes data cleaning steps and analyzes sales trends by city, product category, payment method, gender, and time periods (month/year).

# Store Sales Analysis

## Description
This repository contains a Jupyter Notebook (`sales_data_EDA.ipynb`) that performs data cleaning, exploratory data analysis (EDA), and visualization on a store sales dataset (`techwave_sales.csv`). The analysis aims to uncover trends and insights related to sales performance across different dimensions like location, product categories, customer demographics, payment methods, and time.

## Dataset
The analysis uses the `techwave_sales.csv` dataset, which includes the following key columns (after initial cleanup):
* `Order_Date`: The date the order was placed.
* `Gender`: Gender of the customer.
* `Product_Category`: Category of the product sold.
* `Product_Name`: Specific name of the product sold.
* `Quantity`: Number of units sold.
* `Price`: Price per unit.
* `Total_Sales`: Total sales value for the order line (Quantity * Price).
* `City`: City where the sale occurred.
* `Payment_Method`: Method used for payment.

*(Note: `Customer_ID` and `Order_ID` were dropped during preprocessing).*

## Analysis Performed
The notebook covers the following steps:
1.  **Data Loading:** Importing the dataset using Pandas.
2.  **Initial Cleaning:** Dropping irrelevant columns (`Customer_ID`, `Order_ID`).
3.  **Data Type Conversion:** Converting `Order_Date` to datetime objects.
4.  **Handling Missing Values & Duplicates:** Identifying and removing rows with missing data (`NaN`) and duplicate entries.
5.  **Exploratory Data Analysis & Visualization:**
    * Analyzing total sales per city.
    * Identifying top-performing product categories by sales.
    * Finding the top 5 best-selling products by sales value.
    * Comparing total sales between genders.
    * Analyzing the frequency and total sales value of different payment methods.
    * Extracting `month` and `year` from the `Order_Date`.
    * Analyzing total sales trends across months.
    * Analyzing total sales trends across years.
    * (An additional `city_sales` percentage column was created but not used in the final visualizations shown).

## Tools Used
* Python 3
* Pandas (for data manipulation and analysis)
* Matplotlib (for data visualization)
* Jupyter Notebook (as the development environment)

## How to Run
1.  Clone this repository:
    ```bash
    git clone (https://github.com/saamr6/Store-Sales-Analysis)
    ```
2.  Navigate to the cloned directory.
3.  Ensure you have Python installed, along with the necessary libraries:
    ```bash
    pip install pandas matplotlib notebook
    ```
4.  Make sure the dataset `techwave_sales.csv` is present in the same directory as the notebook.
5.  Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
6.  Open `store analysis.ipynb` and run the cells.

## Results
The detailed analysis, code, and visualizations (bar charts) showing sales trends by city, category, product, gender, payment method, month, and year are contained within the `store analysis.ipynb` notebook.
