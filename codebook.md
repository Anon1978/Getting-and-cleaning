---
title: "codeBook"
author: "Anon Anon Joel"
date: "9 février 2020"
output: pdf_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

--
title: "Untitled"
author: "Anon Anon Joel"
date: "9 février 2020"
output: pdf_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

### CODEBOOK
This project stems from the Coursera Cleaning Data Course. It has 4 weeks of curriculum. In the 4th week, there is an assignment regarding data cleansing. This entire project is based upon the methodology of solving that assignment.
##Tidy data set description

#The variables in the tidy data
Tidy data contains 180 rows and 68 columns. Each row has averaged variables for each subject and each activity.

#Only all the variables estimated from mean and standard deviation in the tidy set were kept.
mean(): Mean value
std(): Standard deviation
#The data were averaged based on subject and activity group.
The dataset includes the following files (some of which are currently too large to upload to this Github repository):

- 'README.txt'  

- 'features_info.txt': Shows information about the variables used on the feature vector.  

- 'features.txt': List of all features.  

- 'activity_labels.txt': Links the class labels with their activity name.  

- 'train/X_train.txt': Training set.  

- 'train/y_train.txt': Training labels.  

- 'test/X_test.txt': Test set.  

- 'test/y_test.txt': Test labels.  
##The following files are available for the train and test data. Their descriptions are equivalent.

'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30.

'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis.

'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration.

'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second.

##Transformation Specifics- 5 functions/requirments and How Source Code run_analysis.R Meets Those Requirements

Merges the training and the test sets to create one data set. Source code "run_analysis.R" loads both test and train data, processes them, and merges the results into one dataset.

Extracts only the measurements on the mean and standard deviation for each measurement. Source code "run_analysis.R" extracts the mean and standard deviation data into one dataset with appropriate column names.

Uses descriptive activity names to name the activities in the data set. Source code "run_analysis.R" loads the descriptive feature and activity labels.

Appropriately labels the data set with descriptive variable names Source code "run_analysis.R" adds appropriately descriptive variable names to the large dataset columns (variables).

From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject Source code "run_analysis.R" calculates the average for all measurement columns grouped by variables Activity and Subject and then writes the output to a local text file named "tidydata.txt""

