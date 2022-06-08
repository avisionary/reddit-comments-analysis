# Project NLP Assignment

## ANLY 502

## Anderson Monken

### Date Given: April 5, 2022

### Due Date: April 15, 2022 11:59 pm

**You should thoroughly read through the entire assignment before beginning your work! Don't start the cluster until you are ready.**

**Data in the cluster's HDFS (Hadoop distributed file system) will be lost when the cluster terminates (CODE AND DATA). If you want to keep data, you must store it in S3.**

## Cluster Setup

1.  Start an EMR cluster as outlined in the Spark guide from this repo with 1 *master* node and 3-7 *core* nodes of `m5.xlarge` instance type up to cluster terminal access. Make sure you use port 8765 for local port forwarding and that you use ssh agent forwarding so that you can push files to GitHub!

2.  Set up your git credentials using the suggested commands in the terminal.

3.  Confirm Git access is set up by running the command `ssh git@github.com`

4.  Clone this repository to the master node by running the command `git clone <repo ssh url>`

5.  Log into Spark according to the steps outlined in the included html file.

6.  Git add, commit, and push your notebook(s)

## Assigment Details (70 points)

This assignment is worth 70 points or about 2 regular homework assignments. Thus, I expect you to put ***significant*** effort into this assignment.

In this assignment you will leverage your PySpark NLP skills to construct textual features from your subreddit data as well as further explore and analyze your text data. You will develop your NLP notebook(s) using PySpark. All your big data analysis must be in PySpark. You may choose to put all your work into one notebook or you may choose to separate it. Either is fine!

REMEMBER!! All the output you are making MUST MUST MUST be small data. Can you make a graph of all 1 million + rows of Spark data? Is it easy to trial and error when using too much data? NO! You MUST MUST MUST take that big data and appropriately use smaller pieces of it as you develop. When you are ready to make outputs, think about how to collapse the data into reasonable types to put into a table or a graph. You should never collect more than \~10,000 rows back to you. This means appropriate aggregations, distributional stats, etc.

Minimum requirements:


-   Conduct basic data text checks / analysis on your data. What are the most common words in general? What is the distribution of text lengths? What are important words according to TF-IDF?

-   Identify important keywords for your subreddit and use regex searches to create dummy variables to identify comments of particular topics.

-   Clean your text data using jonsnowlabs sparkNLP. Think about a few standard procedures to use: stop words, stemming, lemmatizing, removing unusual characters, matching synonyms, etc. You must do at least two of these procedures.

-   Build at least one sentiment model using the sparkNLP framework. Pick a pre-trained model or train your model! You can start off with simple pos/neg/neu sentiment. Maybe you will want to build your own textual classification model.... that is completely up to you and your topical interests and technical goals. You must report a table of summary statistics from the model(s).

-   Produce at least 2 interesting graphs about your resulting dataset. Think about the dimensions that are interesting for your subreddit! There are millions of choices. Make sure your graphs are connected to your business questions.

-   Produce at least 2 interesting tables about your resulting dataset. You can decide how to split up your data into categories, time slices, etc. There are infinite ways you can make summary statistics. Be unique, creative, and interesting!

-   You must save your final dataset in parquet format into your S3 bucket. This will allow you to more quickly work on your next assignment focused on ML without having to re-run any of your transformations.

#### Portfolio Update

You will make the following additions to your website:

1. Natural Language Processing Landing Page

You will populate the NLP page of your project portfolio website. The format should be easy to access, but the method used could be Rmarkdown, HTML, etc. The page will contain the following:

* Part A: an executive summary consisting of 1-2 text paragraphs on your NLP accomplishments. You can include up to 2 images or tables. This is the section to describe the high-level results and the most important information only! This summary must be NON-TECHNICAL! Think about how to touch on your business goals without going into much detail.
    
* Part B: a data analysis style report of 4-7 text paragraphs (each paragraph at least 4 sentences). This is where you will discuss your NLP work and present all your tables and figures. You can save the images or take snips from your Jupyter notebook. This part is for you to write up the analysis work you have already done. Be creative, be awesome!! Show off to a future employer your amazing data science skills!

    * The flow of the report is up to you. Maybe you want to split the text by business goal or organize the prose into a data journey story.
    * You must reference all the business goals that you have accomplished in this report. Did your technical proposal change as you started working with the data?
    * If you made changes to your business goals, discuss your analytical justification for changing your plans. It is OK that plans change, though it is important to describe why.
    * Your graphs must follow the visualization best practices you are learning in ANLY 503. There should be titles, axis labels, legends as needed, etc.

* Part C: Include links to all your coding notebooks (see part 2) and sources for your external data so that your audience can look at your work.

2. Exploratory Data Analysis Coding Notebooks

You will export your .ipynb notebooks to HTML so that you can include them directly in your portfolio website. These will be the notebooks you link in section 1 part C. Make sure you follow good practice of providing markdown titles, subtitles, author information, section headers, comments in your code, etc.

## Submitting the Assignment

You will follow the two part submission process for all labs and assignments:

1.  Add all your requested files to the GitHub assignment repo for the appropriate deliverable
2.  Submit the URL for your repo to Canvas indicating that you have completed your deliverable. **Do not change your GitHub repo after submitting your URL on Canvas**

Make sure you commit **only the files requested**, and push your repository to GitHub!

The files to be committed and pushed to the repository for this assignment are:

-   `README.md`
-   `.gitignore`
-   one or more jupyter notebooks
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
