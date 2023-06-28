# WP42
A wiki repository for the Work Package 4 Task 2 - Statistical/ML-based post-processing methods. Please do not modify this page and go to the [wiki tab instead](https://github.com/DEODE-NWP/WP42/wiki/).

## Guidelines/Checklist for deliverables for WP4

* Ask for access on our DEODE github (https://github.com/DEODE-NWP) to Jonathan Demaeyer and provide your github handle (e.g. @jodemaey).
* Create your own repository for your contributions  **in the DEODE-NWP organization** (one per application/method).
* **By default make your code repositories private, the decision to make it public should be discussed with the managers.**
* Add your repository link and short description to the task wiki home page, e.g. for task 1 on https://github.com/DEODE-NWP/WP41/wiki .
* **Mandatory naming convention for the contributions:** all the code repositories must start with the work package id they belong to, i.e. a code for work package 2 must start with “WP42-” then additional identifiers and then finally the name of the application/method can be added, separated by hyphens ‘-’. For example, assuming that a member-by-member postprocessing code would be added to task 2 contributions, it should be named ‘WP42-methods-MBM’ or ‘WP42-MBM’. It is up to task managers to decide and manage if additional identifiers are needed.
* Code can be developed across several branches in a single code repository, with at least one master/main branch supposedly holding the stable code of the application/method. 
* **When the code is ready and matches the requirement of a deliverable, create a specific branch in the repository holding the code needed and name it ‘WP4n-Deliverable-i’. Lock the branch on Github to block any further development. You can then proceed to continue the work on other deliverables in the other development branches.**
* Describe your case studies as exhaustively as needed in your repositories. Descriptions should include the motivation, data description, your models and method(s), results (outputs and verification) and an outlook.
* Upload your documented code there. The more frequently the better, in order to track your progress.
* Provide a short document (1-2 pages) summarizing the case study for the final, official delivery document. However, more detailed descriptions and results should be referred to the code repositories where all in-depth information have to be available.
* If you want to share small pieces of code with others, please use the “sandbox” of each task, e.g. the sandbox of task 2 is WP42-sandbox: https://github.com/DEODE-NWP/WP42-sandbox . In each sandbox, you can create a new directory and add your code there. Please also add a description in the list in the README of the sandbox.
* If you do not know where your code should belong, you can put it first in the sandbox. 
* You are free to create new pages on the task wikis to discuss technical issues or add additional notes. **Please do not add code to the wiki repositories**.

## Guidelines for containerization for WP4

These guidelines are provisional and may still evolve during the project.
We request the app developpers of the Work Package 4 to abide to these guidelines:

* Document your code as much as possible, this will facilitate the work of the team in charge of containerization.
* In particular, document and identify clearly the inputs and outputs of your code.
* List the dependencies and requirements of your code explicitely in the documentation.
* Allow the location of the data (inputs, outputs, internal data) to be configurable inside your code, e.g. parameterized by some internal or environment variables.
* Document and list the *launch calls* of your code/application, i.e. the command lines which put your app into action. This can for example be a single call to a script, or multiple scripts, or a script with many different possible arguments.
* Link launch calls to inputs and outputs, allowing users to identify which call does what.

An example of a successful containerization is provided [here](https://github.com/DEODE-NWP/WP41-containers-task3-Surge-ThreshPB).
