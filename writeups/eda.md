# Project EDA Assignment

## ANLY 502

## Anderson Monken

### Date Given: March 21, 2022

### Due Date: April 1, 2022 11:59 pm

**You should thoroughly read through the entire assignment before beginning your work! Don't start the cluster until you are ready.**

**Data in the cluster's HDFS (Hadoop distributed file system) will be lost when the cluster terminates (CODE AND DATA). If you want to keep data, you must store it in S3.**

## Cluster Setup

1.  Start an EMR cluster as outlined in the Spark guide from this repo with 1 *master* node and 3-7 *core* nodes of `m5.xlarge` instance type up to cluster terminal access. Make sure you use port 8765 for local port forwarding and that you use ssh agent forwarding so that you can push files to GitHub!

2.  Set up your git credentials using the suggested commands in the terminal.

3.  Confirm Git access is set up by running the command `ssh git@github.com`

4.  Clone this repository to the master node by running the command `git clone <repo ssh url>`

5.  Log into Spark according to the steps outlined in the included html file.

6.  Git add, commit, and push your notebook(s)

## Submission Details (70 points)

You will use the file `project_starter_script.ipynb` to get your subreddit data pulled from the central bucket to your personal bucket. You will develop EDA notebook(s) using PySpark. All your big data analysis must be in PySpark. In this assignment you will examine the dataset, make transformations of the data, produce summary statistics and graphs of the data, and answer some of your business goals that only require exploratory work. You may choose to put all your work into one notebook or you may choose to separate it. Either is fine!

REMEMBER!!! All the output you are making MUST MUST MUST be small data. Can you make a graph of all 1 million + rows of spark data? NO! You MUST MUST MUST take that big data and collapse it into reasonable data to put into a table or a graph. You should never collect more than \~10,000 rows back to you.

Minimum requirements:

-   Report on the basic info about your dataset. What are the interesting columns? What is the schema? How many rows do you have? etc. etc.

-   Conduct basic data quality checks! Make sure there are no missing values, check the length of the comments, remove rows of data that might be corrupted. Even if you think all your data is perfect, you still need to demonstrate that with your analysis.

-   Produce at least 5 interesting graphs about your dataset. Think about the dimensions that are interesting for your subreddit! There are millions of choices. Make sure your graphs are connected to your business questions.

-   Produce at least 3 interesting summary tables about your dataset. You can decide how to split up your data into categories, time slices, etc. There are infinite ways you can make summary statistics. Be unique, creative, and interesting!

-   Use data transformations to make AT LEAST 3 new variables that are relevant for your business questions. I cannot be more specific because this really depends on your project and what you want to explore!

-   Implement regex searches for specific keywords of interest to produce dummy variables and then make statistics that are related to your business questions. Note, you DO NOT have to do textual cleaning of the data at this point. The next assignment on NLP will focus on the textual cleaning and analysis aspect.

-   Find some type of external data to join onto your subreddit data. Don't know what to pick? Consider a time-related dataset. Stock prices, game details over time, active users on a platform, sports scores, covid cases, etc., etc. While you may not need to join this external data with your entire dataset, I want to see at least one analysis that connects to external data.

-   If you are planning to make any custom datsaets that are derived from your subreddit, make them now. These datasets might be graph focused, or maybe they are time series focused, it is completely up to you!

This assignment is worth 70 points. Thus, I expect you to put ***significant*** effort into this assignment. There will also be an associated discussion post that focuses on a website deliverable for EDA. This assignment only requires the Jupyter notebooks.

## Submitting the Assignment

You will follow the two part submission process for all labs and assignments:

1.  Add all your requested files to the GitHub assignment repo for the appropriate deliverable
2.  Submit the URL for your repo to Canvas indicating that you have completed your deliverable. **Do not change your GitHub repo after submitting your URL on Canvas**

Make sure you commit **only the files requested**, and push your repository to GitHub!

The files to be committed and pushed to the repository for this assignment are:

-   `README.md`
-   `.gitignore`
-   `project_starter_script.ipynb`
-   `project_eda.ipynb`
-   `spark_guide.html`

## Grading Rubric

If your the submission meets or exceeds the requirements, is creative, is well thought-out, has proper presentation and grammar, and is at the graduate student level, then the submission will get full credit. Otherwise, partial credit will be given and deductions may be made for any of the following reasons:

Points will be deducted for any of the following reasons:

-   The instructions are not followed
-   There are missing sections of the deliverable
-   The overall presentation and/or writing is sloppy
-   There are no comments in your code
-   There are files in the repository other than those requested
-   There are absolute filename links in your code
-   The repository structure is altered in any way
-   Files are named incorrectly (wrong extensions, wrong case, etc.)
