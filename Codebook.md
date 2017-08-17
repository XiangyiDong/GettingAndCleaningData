# Description

Additional information about the variables, data and transformations used in the course project for the Johns Hopkins Getting and Cleaning Data course.

# Data Set Information

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.
The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

# Merges the training and the test sets to create one data set

trainSet: data from the training set. It contains 7352 observations of 561 features.
testSet: data from the test set. It contains 2947 observations of 561 features.
mergeSet: data contains both training set and test set, resulting 10299 observations of 561 features.
trainLabels: label which kind of activity (1, 2, 3, 4, 5, 6) each row of trainSet corresponds to. It contains 7352 observations.
testLabels: label which kind of activity (1, 2, 3, 4, 5, 6) each row of testSet corresponds to. It contains 2947 observations.
mergeLabel: merge the trainLabels and testLabels, resulting 10299 observations.
subjectTrain: subject# indicates each row of trainSet corresponds to which subject. It contains 7352 observations. Range of subject# are [1, 30]
subjectTest: subject# indicates each row of testSet corresponds to which subject. It contains 2947 observations. Range of subject# are [1, 30]
mergeSubject: merge subjectTrain and subjectTest, resulting 10299 observations.

# Extracts only the measurements on the mean and standard deviation for each measurement

features: contain names of 561 features.
ind: indexes indicate which rows of features correspoding to the measurements on the mean and standard deviation.
mergeSet: selected data which contains the measurements on the mean and std from the original mergeSet.
