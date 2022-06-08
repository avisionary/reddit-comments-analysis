# Project Final Portfolio

## ANLY 502

## Anderson Monken

### Date Given: April 12, 2022

### Due Date: May 3, 2022 11:59 pm

## **CANNOT BE LATE**

**You should thoroughly read through the entire assignment before beginning your work! Don't start the cluster until you are ready.**

**Data in the cluster's HDFS (Hadoop distributed file system) will be lost when the cluster terminates (CODE AND DATA). If you want to keep data, you must store it in S3.**

## Cluster Setup

1.  Start an EMR cluster as outlined in the Spark guide from this repo with 1 *master* node and 3-7 *core* nodes of `m5.xlarge` instance type up to cluster terminal access. Make sure you use port 8765 for local port forwarding and that you use ssh agent forwarding so that you can push files to GitHub!

2.  Set up your git credentials using the suggested commands in the terminal.

3.  Confirm Git access is set up by running the command `ssh git@github.com`

4.  Clone this repository to the master node by running the command `git clone <repo ssh url>`

5.  Log into Spark according to the steps outlined in the included html file.

6.  Git add, commit, and push your notebook(s)

## Assignment Details (90 points)

In this assignment you will complete your portfolio, making sure that it is **ready for primetime**. This means that your portfolio website has been improved since your intermediate assignments and will wow any future employers.

Remember, all your big data analysis must be in PySpark. You may choose to put all your work into one notebook or you may choose to separate out your final work. It might be the case that you have to do very little additional coding for your final portfolio. This really depends on the status of your existing project work and how much more effort you have to put into building it out to be great! More refinement is always better! Iteration always helps! Keep improving the project!

Portfolio requirements:

-   Adapting feedback and making improvements. As part of the revise and resubmit discussion, you are required to make improvements to your project based on prior feedback. You will get more feedback after that point in the semester so that you can improve your project further. This is essential!!!

-   Spell check, grammar check, read for clarity! Make sure all your pages are well-written and free of errors!

-   Submit all your notebooks used in the project to the Git repo! You must also have all your notebooks available on your website!

-   **Introduction page**

    -   You will write up an introduction for your entire project of at least 4 text paragraphs and 2-5 informative graphs/images/tables.

    -   This is a NON-TECHNICAL introduction! There should be no technical language, equations, etc. Talk about what the project, its goals, and why it matters!

    -   All your business goals and technical proposals must be listed out at the end as an appendix to your introduction.

    -   Adapt your project plan discussion post based on any feedback and the changes you have made to your project since you started.

-   **EDA, NLP, and ML pages**

    -   Expand on your analysis from the intermediate assignments in some manner. Do you add an additional data transformation? Try one more model? Try a different NLP text method? It does not have to be groundbreaking at this point, but think about how you can make minor updates to improve the work further.

    -   Improve usability of your pages by fixing issues with html, placement, blurry graphics, etc.

    -   Strengthen the analytical justification of the decisions you made in your project. This text is critical so the audience understands why you followed the path of work that you did.

-   **Conclusion page**

    -   You will write up 3-5 text paragraphs with 2-5 informative graphs/images/tables that summarize and conclude on all the existing work you have done in the project,

    -   You must have a section that discusses next steps in the project. It does not mean that you will actually implement these next steps, but it is important to see your vision for how you would move the project forward.

    -   Make sure you are **not** repeating yourself from the methods pages. If you want to move your summary from methods to conclusion that is OK!

    -   The introduction and conclusion should serve as book ends to your project. If I read them without any of the middle pages, I should still be able to understand the purpose of the project, its impact, and your next steps.

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
