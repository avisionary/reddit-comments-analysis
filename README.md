# Reddit Comments Analysis

## Author : Avi Arora

Visit https://aviarora.georgetown.domains/reddit_analysis/Pages/Introduction.html for detailed information.

## Cluster Setup

1.  Start an EMR cluster as outlined in the Spark guide from this repo with 1 *master* node and 3-7 *core* nodes of `m5.xlarge` instance type up to cluster terminal access. Make sure you use port 8765 for local port forwarding and that you use ssh agent forwarding so that you can push files to GitHub!

2.  Set up your git credentials using the suggested commands in the terminal.

3.  Confirm Git access is set up by running the command `ssh git@github.com`

4.  Clone this repository to the master node by running the command `git clone <repo ssh url>`

5.  Log into Spark according to the steps outlined in the included html file.

6.  Git add, commit, and push your notebook(s)

## Project

In this assignment you will complete your portfolio, making sure that it is **ready for primetime**. This means that your portfolio website has been improved since your intermediate assignments and will wow any future employers.

Remember, all your big data analysis must be in PySpark. You may choose to put all your work into one notebook or you may choose to separate out your final work. It might be the case that you have to do very little additional coding for your final portfolio. This really depends on the status of your existing project work and how much more effort you have to put into building it out to be great! More refinement is always better! Iteration always helps! Keep improving the project!

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


