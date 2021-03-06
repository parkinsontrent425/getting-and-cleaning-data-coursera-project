## Getting and Cleaning Data Course Project

The purpose of this project is to demonstrate the ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis.

### This repository contains the following:

- `README.md` provides an overview of the project and data set.
- `CodeBook.md` describes the conents of the data set (data, variables, and transformations).
- `run_analysis.R` an R script that was used to download the original data and create the `tidy_data.txt`.
- `tidy_data.txt` contains the final data from `run_analysis.R`.

Please see `CodeBook.md` for details pertaining to the variables and transformations on `tidy_data.txt`.

### Study Design

The original data set was obtained from the UCI Machine Learning Repository [Human Activity Recognition Using Smartphones Data Set](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones), which describe how the data was initially collected as follows:

>The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 
>
>The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

### Notes

`run_analysis.R` was run on Windows 10 64-bit edition using R version 3.4.2.

The script require the `data.table` package (version 1.10.4.3 was used) and `plyr` package (version 1.8.4 was used).