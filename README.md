# Getting-and-Cleaning-Data-Course-Project
Getting and Cleaning Data / Course Project

SCRIPT WORKING:-

 STEP 1: Read data from "UCI HAR Dataset"  1)activity_labels.txt and 2)features.txt 
      -- Used read.table()
      
 STEP 2: Read TEST folder files 1) subject_test.txt , 2) X_test.txt and 3) Y_test.txt
      -- Used read.table()
      
 STEP 3: Read TRAIN folder files ,1) subject_train.txt ,2) X_train.txt and 3) Y_train.txt
      -- Used read.table()
      
 STEP 4: ROW BIND simillar data from TEST and TRAIN folders
	X_test with X_train
	Y_test with Y_train
	subject_test with subject_train
	   -- Used rbind()
	   
STEP 5: CHANGING COLUMN NAMES
	Rename Columns of X with names from features.txt file		
	Rename Column  of Y as "Activity_Name"
	Rename Column  of ST as "Volunteer_ID"
     --Used names() function to get column names and replace them with desired names

 STEP 5: Change ROW Values of Y data frame as mentioned in "activity_labels.txt"
	1 - WALKING ,2 - WALKING_UPSTAIRS ,3 - WALKING_DOWNSTAIRS
	4 - SITTING,5 - STANDING, 6 - LAYING
	   -- direct replacement of matched rows with list from "activity_labels.txt"
	
 STEP 6: Filter the MEAN and STANDARD DEVIATION columns from X dataset and create new data set "X_MeanAndStd_Cols"
     --Used grep() function to filter column names that have words, mean() or std() in them
     
 STEP 7: COLUMN BIND Subject, X and Y data sets to form MergedDF data set Order it by Volunteer ID and Activity name columns
      -- Used cbind() to merge the columns and
      -- with() and order() functions to order them by Volunteer ID and Activity(one among 6 in step 5)
      
 STEP 8: FIND MEAN of each variable for each act ivity(Activity_Name) and each subject (Volunteer_ID)
	Write the data set to R workign directory as TidyDataSet.txt
	    --Used aggregate() function to find mean of all other columns 




