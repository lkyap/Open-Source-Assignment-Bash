# CITS4407 Open Source Tools and Scripting - Assignment 2:

## Introduction
- The assignment consists of 2 parts which are (i) data cleaning (ii) data analysis
- There are 2 Shell scripts, prompts.pdf, git_backup, and a README.md in the folder
- The datasets provided in assignment has been taken from Kaggle
- The input dataset for Task 1: data cleaning is "trending_videos_unclean.csv"
- The input dataset for Task 2: Data Analysis is "trending_videos_clean.csv"

## Components in the folder
1. clean
-  This script is for Task 1: Data cleaning
-  It runs few error checks such as "No input file specified", "Input file not found in current directory", "Input file is not CSV", and etc before the cleaning starts.
-  The scripts did the few cleaning processes as following:
  - Delete "ratings_disabled" column
  - Delete rows that contain any empty fields (This include rows do not have video_id)
  - Delete rows which contain 0 likes or dislikes (Rows with both likes and dislikes non-zero are kept)
  - Remove time data from the publish_date column.

2. analyse
- This script is for Task 2: Data Analysis
- It performs the following task:
  - Find the videos that has/have most occurrences
  - Calculate the mean of number of views
  - Find the video(s) that has/have maximum dislikes
  - Find the videos(s) that has/have highest engagement rate. Engagement Rate = (likes + dislikes) / views
  - Find the video(s) that has/have least net sentiment rate. Net sentiment rate = (likes - dislikes) / views

 3. prompts.pdf
- Log of AI prompts used to complete the assignment.

4. git_backup
- Folder contains all data relevant to Git.

## Assumptions make to complete the assignment
1. On data cleaning
- The cleaning order does not matter as mentioned in the discussion post. 

2. On data analysis
  - There will not have duplicated rows on publish date, views, likes and dislikes.
  - Views will always greater than 0 as there will always at least 1 view when the likes and dislikes are always greater than 0 (We have removed the 0 likes or 0 dislikes in Task 1)

