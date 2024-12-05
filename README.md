# Getting and Cleaning Data Project

## Project Overview
This project demonstrates the ability to collect, clean, and prepare tidy data that can be used for future analysis. The dataset used is the UCI HAR Dataset, which includes data from the accelerometers on the Samsung Galaxy S smartphone.

---

## Files in This Repository
- `run_analysis.R`: Script that performs the data cleaning and generates the tidy dataset.
- `final_tidy_data.txt`: Final tidy dataset created by the script.
- `CodeBook.md`: Describes variables, transformations, and processes applied to the dataset.

---

## How to Run the Analysis
1. Download the UCI HAR Dataset from [this link](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip).
2. Extract the dataset and place the folder in your working directory.
3. Place the `run_analysis.R` script in the same working directory.
4. Run the script:
   ```R
   source("run_analysis.R")
