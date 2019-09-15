# 732A54-Big-Data-Analytics

# Lab1-Spark

In this set of exercises you will work exclusively with Spark. This means that in your programs,
you only need to create the SparkContext .In a number of exercises you will be asked to calculated temperature 	averages (daily and monthly). These are not always computed according to the standard definition of ‘average’. In this domain the daily average temperature is calculated by averaging the daily measured maximum and the daily measured minimum temperatures. The monthly average is calculated by averaging the daily maximums and minimums for that month. For example, to get the monthly average for October, take maximums and minimums for each day, sum them up and divide by 62 (which is the same as taking the daily averages, summing them up and divide by the number of days).


# Lab2-Spark SQl
Redo the exercises BDA1 using Spark SQL. An introduction of Spark SQL can be found here
(https://www.ida.liu.se/~732A54/lab/SparkSQLQuickIntro.pdf.)

There are two ways to write queries in Spark SQL - using built-in API functions or running SQL-like
queries. Topassthislab,youneedto:
* use built-in API functions for all the questions
* write a regular SQL query for the second question



# Lab3-Machine Learning with Spark
Implement in Spark1 (PySpark) a kernel method to predict the hourly temperatures for a date and place in Sweden. To do so, you should use the files temperature-readings.csv and stations.csv. Specifically, the forecast should consist of the predicted temperatures from 4 am (04:00) to 12 am (00:00) in an interval of 2 hours for a date and place inSweden.

Use a kernel that is the sum ofthree Gaussian kernels:
* The first to account for the distance from a station to the point of interest.
* The second to account for the distance between the day a temperature measurementwas made
and the day of interest.
* The third to account for the distance between the hour of the day a temperature measurement
was made and the hour of interest.

Choose an appropriate smoothing coefficient or width for each of the three kernels above.You donot need
to use cross-validation.