## Code Book
This document describes the code inside run_analysis.R.

The code is splitted (by comments) in some sections:

- Get the data.
- Read the data from targeted files.
- Merge the test sets to create one dataset.
-Extracts only the measurements on the mean and standard deviation for each measurement
- Uses descriptive activity names to name the activities in the data set.
- Appropriately labels the data set with descriptive variable names.
- Creates a second,independent tidy data set and ouput it.


## Get Data:

Download the file and put the file in data folder. unzip the file

## Read data from targeted files:

Read data from activity, subject and features files into variables.

## Merge the test sets to create one dataset:

Concatenate data tables by rows. Than set names to variables and merge columns to get all data in data frame Data.

## Extracts only the measurements on the mean and standard deviation for each measurement:

Extracts only the measurements on the mean and standard deviation for each measurement. Subset the data frame Data by selected names of Features.

## Uses descriptive activity names to name the activities in the data set:

Read descriptive activity names from “activity_labels.txt”. The activity field in Data is originally of numeric type. We need to change its type to character so that it can accept activity names. The activity names are taken from ActivityLabels.

## Appropriately labels the data set with descriptive variable names:

Names of Features will labelled using descriptive variable names.

## Creates a second,independent tidy data set and ouput it

A second, independent tidy data set will be created with the average of each variable for each activity and each subject based on the previous dataset.