Objective: Practice creating branches for feature development, merging branches, and resolving merge conflicts to simulate a common collaborative workflow on Git and GitHub.

Skills Practiced:

Branching and navigating between branches
Making changes in different branches and committing those changes
Merging branches and resolving conflicts
Task Steps:

Initial Setup:

Use the GitHubCloneProject repository created in the previous task. Create a README.md file if you don’t already have one.
Make sure you have some content in the README.md. You can put in the README file the objective of this task.
Clone the repository to your local machine if you haven’t already:
 git clone <REPOSITORY-URL>
Navigate into the repository’s directory:

 cd GitHubCloneProject
Create a New Branch for a Feature:

Create and switch to a new branch named feature-greeting:
 git checkout -b feature-greeting
Create a new file named feature.txt and add some content related to a feature, for example:

 This is a new feature.
Add and commit the change:

 git add feature.txt
 git commit -m "Add feature description"
Modify the README.md file by adding a new line just below the first line (Second line in the file):

 Modification in feature-greeting branch.
Commit the change:

 git add README.md
 git commit -m "Modify README in feature-greeting branch"
Push the new branch to github (hint: Feel free to google it’s part of learning)
Make Changes in the Main Branch:

Switch back to the main branch:
 git checkout main
Modify the README.md file by adding a new line just below the first line (Second line in the file):

 Modification in main branch.
Commit the change:

 git add README.md
 git commit -m "Modify README in main branch"
Merge the Feature Branch and Resolve a Conflict:

Attempt to merge feature-greeting into main:
 git merge feature-greeting
If a merge conflict occurs, open the conflicting file(s) in a text editor. Manually resolve the conflicts by editing the file to keep or integrate both sets of changes.
After resolving the conflict, add the file to the staging area and commit the merge:

 git add .
 git commit -m "Resolve merge conflict between main and feature-greeting"
Push Changes to GitHub:
Push the updated main branch, including the merged feature and resolved conflict, to GitHub:

 git push origin main
Expected Outcome:

You will have successfully created a new feature branch, made changes in both the feature-greeting and main branches, and resolved a merge conflict resulting from attempting to merge these branches. Your GitHubCloneProject repository on GitHub will reflect these changes and the merge resolution.

Notes:

This project simulates a collaborative scenario where changes made in different branches can lead to conflicts. It tests your ability to manage branches, navigate merge conflicts, and maintain a clean project history.
Replace <REPOSITORY-URL> with your repository’s actual URL.
Repo:

GitHub repository: GitHubCloneProject
File: feature.txt, README.md