\# Git Practice Project Task 2

This is the descriptive readme for assignment 1, task 2, SER316 ONLINE



Initial Branches and Commits:



Dev: This adds an encouraging "Good Luck" message as the only change from Main. 2 commits, initial and message. This will have conflicts.



Main: This contains the initial program, tested, with no additional features and only the initial commit. No conflicts from this branch likely.



Hotfix: This contains the program with from main with a fix for Utils and tests for UtilsTest. 2 commits, initial and fix. Conflicts expected with line overlap.



Documentation: Made by me, contains the readme you're reading. Has a commit for that. No conflicts expected. 



Feature1: Starts with Main, adds quit game feature in first commit, play again loop in second commit, improves feedback in third commit, 

and adds version comment in the fourth commit. Plenty of conflicts anticipated.

&nbsp;

Feature2: Starts with main, adds same good luck message as dev (conflict) in first commit, adds maxAttempts constant and gameOver state in second commit,

and implements max attempts and game over conditions in third commit. Conflicts expected.



Feature3: Starts with main, adds hints over four poorly messaged commits that could've been one or one with hotfixes. Conflicts expected.

Learning Summary:

Differences between merge, rebase, squash, and cherry-pick:

Merge: Merge takes multiple branches and combines them into one new merge commit with two parent commits.
This preserves the branch histories and shows clearly where they were merged. Conflicts are dealt with all at once.

Rebase: Rebase takes one branch and layers it onto a target branch, applying commits one by one on top of the target 
branch's commits. This rewrites the two histories into one shared history that is linear and easier to follow, avoiding
extra unnecessary merge commits (when appropriate). This is very risky with shared repos.

Squash: Takes multiple commits and consolidates them into one commit. Creates a more readable and concise history. This
allows for easier collaboration, and easier reverts if necessary.

Cherry-pick: Taking one specific commit from a branch and applying it to another branch, rather than doing a full merge.
This allows you to selectively apply commits that are necessary and ignore what's not.

Git History: Feature1 and Feature2 had more typical git histories, while feature3 was obviously intentionally poorly 
commented. After squashing feature3 into a concise history, the flow of git history is uniform and easy to follow.
Feature1 is no longer available in the repo but it's history has been incorporated into the updated work.

When to use each strat in real projects:
Merging is going to be used very frequently whenever working on real projects in order to sync work up and test the 
product. Its how you combine individual work into a whole for the most part, as rebasing is risky with shared repos. 
In an ideal world, we won't have to squash much, but when history is becoming too dense it is always a helpful tool to
have available. Cherry-picking is helpful for partner-programming and if multiple people are working on the same 
issue, as it allows you to take the best parts that work and attach only those to the product. Rebasing is very useful
in local projects, as it is a more linear combination of branches.