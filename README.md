
The project’s purpose is to demonstrate persons ability to collect, work with, and clean a data set with a goal of preparing tidy data that can be used for future analysis. 

run_analysis.R performs the following in this project:

Merging: 
Merges the training and the test sets and creates one single data set.

Extracting:
Extracts only the measurements on the mean and standard deviation for each measurement in the data.

Description:
Uses descriptive activity names to name the activities in the data set

Labelling:
Labels the data set with descriptive activity names.

An independent tidy data set is created with the average of each variable for each activity and each subject.
run_analysis.R

It works by downloading the dataset to working directory, unzips file into the UCI HAR Dataset folder.
Train and test data sets are loaded, appended into one data frame using rbind
Mean and SD are extracted using grep.
Column names are cleaned, applied to the x data frame.
Converts dataset to lowercase and subject column names are named 
Three data sets are merged and exported to txt file into the project folder in the same working directory.
Mean of activities and subjects are created as tidy data set, exported as txt file, named average.txt
R code is with str for easier preview of the two final data sets.
