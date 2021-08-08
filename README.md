## Getting-and-Cleaning-Data-Final-Assignment

Class homepage : https://www.coursera.org/learn/data-cleaning

- Author: jc32569
- No Copyrights, Public Domain, August 2021
- Runnable source script: run_analysis.R

## Task desrciption

(repeated in the source script "run_analysis.R" alongside the actual execution code):

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
6. Please upload the tidy data set created in step 5 of the instructions. Please upload your data set as a txt file created with write.table() using row.name=FALSE
7. Please submit a link to a Github repo with the code for performing your analysis. The code should have a file run_analysis.R in the main directory that can be run as long as the Samsung data is in your working directory. The output should be the tidy data set you submitted for part 1. You should include a README.md in the repo describing how the script works and the code book describing the variables.

### Results

** tidydata.txt -- contains the final tidied output data.

** CodeBook.md -- description of all variables

The description how the result has been achieved is contained within the source file "run_analysis.R".

This can be run as one big batch of instructions from the R console. The only customization proably needed is to set the starting directory. Just search for the line baseDir <- "~/Documents/coursera/getting-and-cleaning-data/assessment-tidy-data" and change it to your environment.

Otherwise the instructions from the R script can be executed and checked step by step for review.

The data source is not included in the git repository. The R script downloads it into subdir named "data" during runtime.

#### Analyzed source data
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

(see below for licensing conditions of the data itself)

#### Notes about data structure:
- "X_train.txt" has 7352 lines with sample values -> 561 columns, described by name in "features.txt" and with more info in "features_info.txt"
- "subject_train.txt" has 7352 lines with coded values for the person (subject)
- "y_train.txt" has 7352 lines with coded values for the activity

The same structure is repeated for test (replace "train" with "test" in file names, 2947 lines with measurement values which are added to the 7352 lines from the training set).




