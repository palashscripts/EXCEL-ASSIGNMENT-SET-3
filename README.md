# Insurance Data Analysis Dashboard


This project involves analyzing insurance data using Excel to create a comprehensive dashboard. The assignment consists of three main tasks:

1. Recording a Macro: Creating new columns for `Total Insured` and `Premium Per Head`.
2. Data Validation: Applying rules to ensure data integrity.
3. Creating a Dashboard: Visualizing the data using charts.

## Data Description

The dataset contains the following columns:
- `age`: The age of the insured person.
- `children`: Number of children covered by insurance.
- `premium / Expenses`: Premium expenses paid by the insured person.
- `gender`: Gender of the insured person.
- `smoker`: Whether the insured person is a smoker (`yes` or `no`).
- `BMI`: Body Mass Index of the insured person.
- `region`: Region where the insured person lives.

## Steps

### Assignment 1: Recording a Macro

1. Create `Total Insured` Column:
   - Formula: `=D2+1` and 1 is our male or female because of the family member (`children` is in column `D` and the first row of data is row 2).
   - Copy this formula down the entire column `H`. Total Insured 

2. Create `Premium Per Head` Column:
   - Formula: `=G2 / H2` (`premium / Expenses` is in column `G2` and `Total Insured` is in column `H`).
   - Copy this formula down the entire column `I`.


### Assignment 2: Data Validation

1. Age Validation:
   - Select the `age` column.
   - Go to `Data` > `Data Validation`.
   - Set criteria: `Whole number` between `18` and `80`.

2. Gender Validation:
   - Select the `gender` column.
   - Go to `Data` > `Data Validation`.
   - Set criteria: `List` with values `male, female, others`.

3. BMI and Expenses Validation:
   - Select the `BMI` column.
   - Go to `Data` > `Data Validation`.
   - Set criteria: `Decimal` greater than `0`.
   - Repeat for the `premium / Expenses` column.

4. Smoker Validation:
   - Select the `smoker` column.
   - Go to `Data` > `Data Validation`.
   - Set criteria: `List` with values `yes, no`.

### Assignment 3: Creating a Dashboard

1. Average Premium Per Head by Age (Line Chart):
   - Create a Pivot Table with `age` in Rows and `Premium Per Head` in Values (set to average).
   - Insert a Line Chart and title it "Average Premium Per Head by Age".

2. Fraction of Male and Female Population Who Smoke (Bar Chart):
   - Create a Pivot Table with `gender` in Rows and `smoker` in Columns and Values (set to count).
   - Insert a Bar Chart and title it "Fraction of Male and Female Population Who Smoke".

3. Count of People Who Smoke in Each Region (Pie Chart):
   - Create a Pivot Table with `region` in Rows and `smoker` in Columns and Values (set to count).
   - Insert a Pie Chart and title it "Count of People Who Smoke in Each Region".

## Files

- `Insurance FIle.xlsx`: The Excel file containing the data and the dashboard.

## Conclusion

This project demonstrates how to perform data analysis and visualization using Excel, ensuring data integrity through validation and automating repetitive tasks with macros.
