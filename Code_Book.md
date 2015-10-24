This file describes what the run_analysis.R script does.

1. First set your working directory
2. Checks whether the folder "UCI HAR Dataset" exists, if the folder 
does not exist a file will be downloaded under the name "UCI HAR Dataset.zip"
3. Then following txt files will be loaded into R:

x_test
y_test
subject_test
x_train
y_train
subject_train
features
activity_labels

4. Check the dimensions of the files loaded onto R
5. Binding the appropriate datasets together.
6. Labelling the datasets' headers. Activity_lables used to label ActivityID which
is the combination of y_test and y_train. Features dataset used to label the fields for combination
of x_test and X_train.
7. Extract only the data that is associated with the calculation of mean and standard deviation of
the variables.
8. Binding all the various data set together to form on large dataset called "Alldata". A txt
will also be created called "merged_Alldata.txt"
9. Creates an independent tidy data set with the average of each variable for each activity 
and each subject. Create a calcualted tidy dataset, and a txt file made called 
"MeanSD_Tidy_Data.txt"

---------------------------------------------------------------------------------------------------------------------

Description of the variables:

- 'features_info.txt': Shows information about the variables used on the feature vector.

- 'features.txt': List of all features.

- 'activity_labels.txt': Links the class labels with their activity name.

- 'train/X_train.txt': Training set.

- 'train/y_train.txt': Training labels.

- 'test/X_test.txt': Test set.

- 'test/y_test.txt': Test labels.

The following files are available for the train and test data. Their descriptions are equivalent. 

- 'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30. 

- 'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis. 

- 'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration. 

- 'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second. 

