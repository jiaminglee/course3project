Read Data
1) First the script reads the data from feature.txt and activity_labels.txt. This are then parsed into featureNames and activityLabels.
2) Data from the respective x_train.txt, y_train.txt, subject_train.txt, x_test.txt, y_test.txt, subject_test.txt are then parsed into subjectTrain, activityTrain, featureTrain, subjectTest, activityTest, featureTest respectively

Part 1 - Merges the training and the test sets to create one data set.
1) The subjectTrain, subjectTest will then be combined into subject
2) The activityTrain, activityTest will then be combined into activity
3) The featureTrain, featureTest will then be combined into feature

Part 2 - Extracts only the measurements on the mean and standard deviation for each measurement. 
1) The mean and standard deviation are then extracted into extractedData

Part 3 - Uses descriptive activity names to name the activities in the data set
1) The activity names are taken from metadata `activityLabels`.

Part 4 - Appropriately labels the data set with descriptive variable names
1) Acc, gyro, body body, mag, f, t, tBody, -mean(), -std(), -freq(). angle, gravity are then replaced properly with Accelerometer, Gyroscope. Body. Magnitude, Frequency, Time, Mean, Std, Frequency, Angle and Gravity. This allows the data set to reflect the proper descriptive names

PArt 5 - Creating independent tidy data set with the average of each variable for each activity and each subject
1) tidy data is created with the average of each variable for each activity and each subject
2) write them into a text file




