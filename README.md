# Getting-and-Cleaning-Data-Course-Project
#
#Data for the project: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
#
#Repository structure: -/"UCI HAR Dataset" all files to run run_analysis.R -README.md this file. -codebook.md description of variables -run_analysis.R R script to produce tidyData.txt -tidyData.txt the file generated by run_analysis.R
#
#How is it run?
#
#- save the complete folder databases in the current working directory of the R process name as "UCI HAR Dataset" in your machine fron https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
#- apply the library "data.table", "reshape2", "dplyr"
#- run run_analysis.R
#- tidyData.txt will be generate in your working directory
#
#What does run_analysis.R do?
#
#- read in the 'Subject' data
#- read in the 'Activity' data
#- read in the 'Measures' data
#- merge the Train and Test Subjects
#- merge the Train and Test Activities
#- merge the Train and Test 'Measures' data
#- merge the subjects to activities
#- order data by, subject and activity
#- read in the 'features.txt'
#- get features/measures related to mean and std
#- take the rows with the columns of interest
#- merge the 'meaningful activity names' with the SubjectActiitiesWithMeasuresMeanStd
#- merge measure codes
#- write the tab delimited file file="tidyData.txt"
