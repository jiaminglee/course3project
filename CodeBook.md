Data from this project is used from
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

This datasets contains data collected from the accelerometers from the Samsung Galaxy S smartphone. 


Input data set

1) Activity_labels.txt has the metadata from the various activities
2) Features.txt contains name of those features

Input data sets are contain in 2 folders namely, “test” and “train”.
Test
1) x_test.txt contains features for testing
2) y_test.txt contains activities relating to x_test.txt
3) subject_test.txt contains info on the subjects that data was collected from

Train
1) x_train.txt contains features for testing
2) y_train.txt contains activities relating to x_test.txt
3) subject_train.txt contains info on the subjects that data was collected from


Formatting the data set
1) x_test, y_test and subject_test are processed into featuretest, activitytest and subjecttest
2) x_train, y_train and subject_train are processed into featuretrain, activitytrain and subjecttrain
3) Both the featuretest and featuretrain are then merged into “features”
4) Both the activitytest and activitytrain are then merged into “activity”
5) Both the subjecttest and subjecttrain are then merged into “subject”
6) All the “features”, “activity” and “subject are then combined and merged into completedata

7) Mean and standard deviation is then extracted into extracted data
8) Appropriately labels the data set with descriptive variable names. This can be seen in the pseudocode.
9) Create tidy data that contains the average of each variable for each activity and each subject.
10) Lastly, write them into a text file
