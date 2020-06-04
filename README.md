# Introduction

## Project Overview
In this project, I created 3 tables in a Cassandra database. A ETL pipeline is employed to collect csv files from a folder, put them in a staging file and insert data in the tables created in Cassandra database.

Since 3 queries is provided for this task, the new created tables answer these queries. 

## Project: Data Modeling with Cassandra
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

# Project Details

## Datasets
For this project, I worked with one dataset: event_data. The directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:

    event_data/2018-11-08-events.csv
    event_data/2018-11-09-events.csv

## Project files
1. event_data/* folder contains raw data in csv files to be analyzed.
2. event_datafile_new.csv is a staging area for data
![event_datafile_new](images/image_event_datafile_new.jpg)
3. Project_1B_Cassandra.ipynb processes the event_datafile_new.csv dataset to create a denormalized dataset
, models the data tables for 3 queries, loads the data into tables and run queries

## 3 Queries
1. Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4
2. Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'



[rubrics](https://review.udacity.com/#!/rubrics/2475/view)
