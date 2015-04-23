

The variables used in the  run_analysis.R are as follows

Features            - Data from UCI HAR Dataset/features.txt
Activities	    - Data from UCI HAR Dataset/activity_labels.txt
TestST	   	    - Data from UCI HAR Dataset/test/subject_test.txt
TestX		    - Data from UCI HAR Dataset/test/X_test.txt
TestY	    	    - Data from UCI HAR Dataset/test/Y_test.txt
TrainST	    	    - Data from UCI HAR Dataset/train/subject_train.txt
TrainX	            - Data from UCI HAR Dataset/train/X_train.txt
TrainY	    	    - Data from UCI HAR Dataset/train/Y_train.txt
ST	    	    - Merged TestST and TrainST dataset
X	    	    - Merged X_Test and X_Train Data set
Y	    	    - Merged Y_Test and Y_Train Data set
Activity_Names	    - Data frame that have the 6 activities from UCI HAR Dataset/activity_labels.txt
MeanCols	    - Data frame with Column Names that have word "mean()" in them
StdCols	    	    - Data frame with Column Names that have word "std()" in them
MeanAndStdCols	    - Data frame that is MeanCols + StdCols
X_MeanAndStd_Cols   - Data frame with MEAN and STD columns ALONE
MergedDF	    - Data Frame that has Subject , X and Y data from both TEST and TRAIN folders
OrderedDF	    - Ordered MergedDF data frame
MeanDF	    	    - Data frame with Activity and Volunteer ID and MEAN of other columns
TidyDF	    	    - Final Data frame with Means
