# Project ML Assignment

## ANLY 502

## Anderson Monken

### Date Given: April 10, 2022

### Due Date: April 23, 2022 11:59 pm

**You should thoroughly read through the entire assignment before beginning your work! Don't start the cluster until you are ready.**

**Data in the cluster's HDFS (Hadoop distributed file system) will be lost when the cluster terminates (CODE AND DATA). If you want to keep data, you must store it in S3.**

## Cluster Setup

1.  Start an EMR cluster as outlined in the Spark guide from this repo with 1 *master* node and 3-7 *core* nodes of `m5.xlarge` instance type up to cluster terminal access. Make sure you use port 8765 for local port forwarding and that you use ssh agent forwarding so that you can push files to GitHub!

2.  Set up your git credentials using the suggested commands in the terminal.

3.  Confirm Git access is set up by running the command `ssh git@github.com`

4.  Clone this repository to the master node by running the command `git clone <repo ssh url>`

5.  Log into Spark according to the steps outlined in the included html file.

6.  Git add, commit, and push your notebook(s)

## Assignment Details (70 points)

This assignment is worth 70 points or about 2 regular homework assignments. Thus, I expect you to put ***significant*** effort into this assignment.

In this assignment you will leverage your PySpark machine learning skills to build models with your subreddit data as well as further explore, clean, and analyze your data. You will develop your ML notebook(s) using PySpark. All your big data analysis must be in PySpark. You may choose to put all your work into one notebook or you may choose to separate it. Either is fine!

REMEMBER!! All the output you are making MUST MUST MUST be small data. Can you make a graph of all 1 million + rows of Spark data? Is it easy to trial and error when using too much data? NO! You MUST MUST MUST take that big data and appropriately use smaller pieces of it as you develop. When you are ready to make outputs, think about how to collapse the data into reasonable types to put into a table or a graph. You should never collect more than \~10,000 rows back to you. This means appropriate aggregations, distributional stats, etc.

Minimum requirements:

-   Construct at least two machine learning analyses using the machine learning libraries in PySpark. First, select a business goal for each of your ML analyses. There MUST be at least two different analyses conducted. For each analysis you will compare two or more models. For each ML analysis, you must follow best practice and apply the following broad steps:

    -   Prepare your data for modeling. Conduct any remaining feature transformations and apply additional textual processing steps to have the needed variables in your data.

    -   Conduct at 2 ML transformations for your data by applying string indexer, vectorizer, or other transformers.

    -   Split data into testing and training if you are running supervised models.

    -   Run at least two models (more is always fine!) on your data. Within each model, you will compare at least 2 different hyperparameter sets.

    -   Run model evaluation metrics (ROC AUC, Confusion Matrix, Accuracy, R2, etc.) on your models and hyperparameter options. There must be at least four outcomes to compare since you will have at least two models with at least 2 different hyperparameter sets each.

    -   Prepare at least 1 appropriate table and at least 1 chart for each ML analysis. You do not need one for every model / hyperparameter set.

-   You must save at least two ML models into your S3 bucket. Demonstrate that you can save your best ML model of each ML analysis and load the prepared model into your notebook and start making predictions without any additional training. This can be done in a separate notebook.

-   **Bonus points (+2 points)**: Apply pipelines for your ML analysis so that you can compare hyperparameters and model options without having to re-run large parts of code.

#### Portfolio Update

You will make the following additions to your website:

1.  Machine Learning Landing Page

You will populate the ML page of your project portfolio website. The format should be easy to access, but the method used could be Rmarkdown, HTML, etc. The page will contain the following:

-   Part A: an executive summary consisting of 1-2 text paragraphs (each paragraph at least 4 sentences) on your ML model outcomes. Your writing must be excellent here and persuasive. 3 sentences total WILL NOT CUT IT! I expect you to write at least 8 sentences. You can include up to 2 images or tables and your text can discuss these images/tables. This is the section to describe the high-level results and the most important information only! This summary must be NON-TECHNICAL! Think about how to touch on your business goals without going into much detail.

-   Part B: a data analysis style report of 4-7 text paragraphs (each paragraph at least 4 sentences). This is where you will discuss your ML prep, execution, and evaluation. During that prose, you will present all your tables and figures. You can save the images or take snips from your Jupyter notebook. This part is for you to write up the analysis work you have already done. Be creative, be awesome!! Show off to a future employer your amazing data science skills!

    -   The flow of the report is up to you. Maybe you want to split the text by business goal or organize the prose into a data journey story.
    -   You must reference all the business goals that you have accomplished in this report. Did your technical proposal change as you started working with the data?
    -   If you made changes to your business goals, discuss your analytical justification for changing your plans. It is OK that plans change, though it is important to describe why.
    -   Your graphs must follow the visualization best practices you are learning in ANLY 503. There should be titles, axis labels, legends as needed, etc.

-   Part C: Include links to all your coding notebooks (see part 2) and sources for your external data so that your audience can look at your work.

1.  Exploratory Data Analysis Coding Notebooks

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
