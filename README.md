# Wrangle and Analyze Data
Udacity Data Analyst Nanodegree program


Wrangle and Analyze Data - WeRateDogs twitter account




# Project Overview
## Introduction

The dataset that I wrangled, analyzed, and visualized is the tweet archive of Twitter user [@dog_rates](https://twitter.com/dog_rates), also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "[they're good dogs Brent](https://knowyourmeme.com/memes/theyre-good-dogs-brent)." WeRateDogs has over 8.7 million followers as of June 15, 2020 and has received international media coverage.

WeRateDogs downloaded their Twitter archive and sent it to Udacity via email exclusively to use in this project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017. 

# <img src="https://cdn10.bostonmagazine.com/wp-content/uploads/sites/2/2017/04/WeRateDogs.jpg" width="500">
## <center>Image via Boston Magazine</center>

## What Software Do I Need?

- The entirety of this project was completed in a Jupyter Notebook. 
- The following packages (libraries) need to be installed. You can install these packages via conda or pip. 
  - pandas
  - NumPy
  - requests
  - tweepy
  - json


# Project Specifications

## Project details
- Data wrangling, which consists of Gathering data, Assessing data, and Cleaning data.
- Storing, analyzing, and visualizing the wrangled data
- Reporting on 1) the data wrangling efforts and 2) the data analyses and visualizations

## Gathering Data for this project
Gather each of the three pieces of data as described below in a Jupyter Notebook titled [wrangle_act.ipynb](---------------------) 
- The WeRateDogs Twitter archive. Udacity gave this file to me, so imagine it as a file on hand. Download this file manually by clicking the following link: twitter_archive_enhanced.csv
- The tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file ( image_predictions.tsv ) is hosted on Udacity's servers and should be downloaded programmatically using the Requests library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_imagepredictions/image-predictions.tsv
- Each tweet's retweet count and favorite ("like") count at minimum, and any additional data which are interested. Using the tweet IDs in the WeRateDogs Twitter archive, query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of JSON data in a file called tweet_json.txt file. Each tweet's JSON data should be written to its own line. Then read this .txt file line by line into a pandas DataFrame with (at minimum) tweet ID, retweet count, and favorite count.



## Assessing Data for this project
1. After gathering each of the above pieces of data, assess them visually and programmatically for quality and tidiness issues:
   - Visual assessment: each piece of gathered data is displayed in the Jupyter Notebook for visual assessment purposes. Once displayed, data can additionally be assessed in an external application (e.g. Excel, text editor).
   - Programmatic assessment: pandas' functions and/or methods are used to assess the data.
2. Detect and document at least eight (8) data quality issues and two (2) tidiness issues in the wrangle_act.ipynb Jupyter Notebook.

## Cleaning Data for this project
- Clean each of the issues you documented while assessing
- Perform this cleaning in wrangle_act.ipynb as well
- The result should be a high quality and tidy master pandas DataFrame

## Storing, Analzing, and Visualizing Data for this projct
- Store the clean DataFrame(s) in a CSV file with the main one named twitter_archive_master.csv 
- Analyze and visualize the wrangled data in wrangle_act.ipynb Jupyter Notebook. 
- Produce at least three (3) insights and one (1) visualization

## Reporting for this project

- Create a written report called wrangle_report.pdf or wrangle_report.html that briefly describes wrangling efforts.
- Create a written report called act_report.pdf or act_report.html that communicates the insights and displays the visualization(s) produced from wrangled data