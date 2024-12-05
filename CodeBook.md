# Code Book for UCI HAR Dataset Analysis

## Overview
This codebook describes the variables, data structure, and transformations used in the "Getting and Cleaning Data" project. The dataset represents data collected from the accelerometers of Samsung Galaxy S smartphones.

---

## Variables

### Subject Information
- **subject**: Identifier for the participant in the study (range: 1-30).

### Activity Information
- **activity**: Descriptive labels for activities performed by participants:
  - WALKING
  - WALKING_UPSTAIRS
  - WALKING_DOWNSTAIRS
  - SITTING
  - STANDING
  - LAYING

### Measurement Variables
Only mean and standard deviation measurements were selected. Here are some examples:
- **TimeBodyAccelerometer-mean()-X**: Mean of body acceleration along the X-axis.
- **TimeBodyAccelerometer-std()-Y**: Standard deviation of body acceleration along the Y-axis.
- **FrequencyBodyGyroscope-mean()-Z**: Mean of body gyroscope along the Z-axis.

### Units
- Measurements are normalized and unitless.
- Subject identifiers are integers.
- Activity labels are categorical.

---

## Transformations
1. Merged the training and test datasets to create one combined dataset.
2. Extracted measurements containing mean (`-mean()`) and standard deviation (`-std()`).
3. Replaced activity codes with descriptive activity names.
4. Appropriately labeled variables with descriptive names:
   - Prefix `t` was replaced with `Time`.
   - Prefix `f` was replaced with `Frequency`.
   - Abbreviations expanded (e.g., `Acc` → `Accelerometer`).
5. Created an independent tidy dataset with the average of each variable for each activity and each subject.

---

## Summary
The final tidy dataset includes:
- 68 columns (subject, activity, and 66 measurements).
- 180 rows (30 subjects × 6 activities).
