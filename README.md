# Getting-and-Cleaning-Data-Assignment
This is the course project for the Getting and Cleaning Data Coursera course.

One of the most exciting areas in all of data science right now is wearable computing - see for example [this article](http://www.insideactivitytracking.com/data-science-activity-tracking-and-the-battle-for-the-worlds-top-sports-brand/). Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users.

In this project, data collected from the accelerometer and gyroscope of the Samsung Galaxy S smartphone was retrieved, worked with, and cleaned, to prepare a tidy data that can be used for later analysis.

This repository contains the following files:

- `README.md`, this file, which provides an overview of the data set and how it was created.
- `tidy.txt`, which contains the data set.
- `CodeBook.md`, the code book, which describes the contents of the data set (data, variables and transformations used to generate the data).
- `run_analysis.R`, the R script that was used to create the data set (see the [Creating the data set](#creating-data-set) section below) 


The R script `run_analysis.R` does the following:

1. Download the dataset if it does not already exist in the working directory.
2. Load the activity and feature info.
3. Loads both the training and test datasets, keeping only those columns which reflect a mean or standard deviation.
4. Loads the activity and subject data for each dataset, and merges those columns with the dataset.
5. Merges the two datasets.
6. Converts the activity and subject columns into factors.
7. Creates a tidy dataset that consists of the average (mean) value of each variable for each subject and activity pair.

The end result is shown in the file `tidy.txt`.
