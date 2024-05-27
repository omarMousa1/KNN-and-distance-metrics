# KNN-and-distance-metrics
The distance metric is used to determine which points in the training dataset are "nearest" to the new data point that we are trying to classify. 


# Introduction
In the k-nearest neighbors (KNN) algorithm, the distance metric is used to determine which points in the training dataset are "nearest" to the new data point that we are trying to classify. The distance metric is used to compute the distance between the new data point and the existing points in the training dataset. The KNN algorithm then selects the K points in the training dataset that are closest to the new data point and classifies the new data point based on the most common class among these K points.

Some common distance metrics that can be used with the KNN algorithm include:

-	Sorensen distance (SD)
  
-	Additive distance (ASCSD)
  
-	Divergence distance (DivD)
  
-	Jaccard distance (JacD)



# Analytics of the datasets we chosen: 
1.	exams dataset : This dataset consists of the marks of the students in various subjects, it evaluates students’ performance in exams.
The original dataset contains 8 columns (attributes)-- [gender, race/ethnicity, parental level of education, lunch, test preparation course, math score, reading score, writing score] and 1001 rows (observations).

2.	diabetes dataset :  This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the dataset is to diagnostically predict whether a patient has diabetes, based on certain diagnostic measurements included in the dataset.
It contains 8 attributes and the class -- [Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age, Outcome(class)] and 769 observations. It is particularly good and there are no problems or columns that should be removed. Most values in all columns are consistent.

3.	covid-19 dataset : Contains a vast amount of anonymized patient-related information including pre-conditions. The raw dataset consists of 21 unique features and 1,048,576 unique patients. In the Boolean features, 1 means "yes" and 2 means "no". values as 97 and 99 are missing data.

In dataset Covid_Data(UP).csv, this data is good, because it contains a     lot of columns with values that we will classification the KNN. There are some columns that contain a string type, such as the dates column, so we removed it. Although data contains about half a million data records, we take the first 1500 data records.

We prepare and clean our dataset exams(UP).csv, there are a lot of numbers and strings, but there were no values to classification the KNN, so we made a simple equation to make males with (1) instead of (‘Male’), and females with (0) instead of (‘Female’).
We removed all columns from type string and kept the columns that have numbers (numeric) because they are basis of the work.
