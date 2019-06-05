# git-p4
Copy of https://git.kernel.org/pub/scm/git/git.git/log/git-p4.py as of 2019-02-05

# Purpose
This repository was created to update the git-p4.py script to properly work with windows.

#Setup
See the tutorial at: https://www.atlassian.com/git/tutorials/git-p4

##New git hooks
A new Git hook  `p4-pre-edit-changelist` has been added.  This will allow editing a changelist prior to presenting it to the user. In our environment, there is certain text required in a submit that must be present.  This hook allows editing the changelist to insert this text.