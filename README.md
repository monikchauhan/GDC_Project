### Getting and Cleaning Data
##### Course Project

You should create one R script called run_analysis.R that does the following.

Merges the training and the test sets to create one data set.
Extracts only the measurements on the mean and standard deviation for each measurement.
Uses descriptive activity names to name the activities in the data set
Appropriately labels the data set with descriptive activity names.
Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

#### Steps to work on this course project

1.  Download the data source and put into a folder on your local drive. You'll have a UCI HAR Dataset folder.
2.  Put run_analysis.R in the parent folder of UCI HAR Dataset, then set it as your working directory using setwd() function in RStudio.
3.  Run source("run_analysis.R"), then it will generate a new file tiny_data.txt in your working directory.

#### Dependencies

 It depends on reshape2 and data.table.

#### How the script works
1. Load test data.
2. Filter data for mean and SD measurements.
3. Gives descriptive variables.
4. Bind subject, y and X test data.
5. Repeat steps 1-4 for train data.
6. Merge test and train data.
7. Create a new tidy data set with the average of each variable for each activity and each subject.
