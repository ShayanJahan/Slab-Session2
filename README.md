# Project

At first, we have added our module "sum.py". We have committed our changes using this line:

git commit -m 'Add sum.py' -m 'This module is going be able to add two numbers and show the result to the user'

After that, we have updated 'README.md',and committed our changes using this line:

git commit -m 'Update README.md' -m 'New information has been added to README'

Next, we make branch main protected, and we make a new branch named dev.

After that, we solve problem for inputs at most 10 in branch dev, and we merge this branch into branch main

Now, we improve the code in branch dev and solve problem for inputs at most 30.

Since we have changed both README.md and sum.py, we want to add and commit them separately. First, we add both of them; then, we undo adding README.md by the following command:

git restore --staged README.md

At the end, we commit both changes seperately.

Now, we want to merge branches dev and main. Since the file 'README.md' is different in these two branches, we must resolve conflicts.

Then, we improve code in branch dev to solve problem for input at most 50. At the same time, in bran dev2, we solve problem for inputs at most 70, and we have a minor bug, we set result = a + b + 1. This way we will have to solve conflicts at the end. This will be our second resolving conflict.

Meanwhile, using commands like 'git log' and 'get diff', we can get necessary informations.

We make a new branch hotfix, and fix the recent bug in this branch. At the end, we merge it into branch main.

Then, we solve problem completely in branch dev by removing if; and we merge it into main using a pull request.

Finally, while we are testing, we add a .gitignore to avoid pushing tests.

# Questions

1. .git folder will save commit history and all other necessary informations for git. In one word, everything that git does, it will do by this folder.

2. The atomicity of commits and pull requests means that they will either be done entirely or nothing will change at all. Also they can be reverted without any side effect.

3. In one word pull = fetch + merge. When we fetch, it pulls all the commits from the remote branch, without merging it. Thus, fetch and merge are safer, and pull faster. For example, when some changes have happened, we can simply pull all of them, or we can first fetch them, and then merge them.

4. The difference between clone and rebase is that rebase will completely modify the project's history. But clone will just copy the project in the remote repository into your local repository. For example, when we want to start working on a project we use clone. And, when we made some changes, and we want to define new history for our projects (for example we made changes on another branch, and we want that to be the history of versions that we have), we use rebase.

5. The command 'git reset' will be used to reset changes on a private branch; which means, using that you can reset uncommitted changes. While the command 'get revert' will be used to reset changes on a public branch; This means you can reset changes committed changes. For example, when you are working on your own local repository, and you made mistake and you want to put everything back to some state, you may use git reverse; on the other hand, when you are working on remote branch and you have made some mistake on the changes you made, you may use git revert to put everything back at their previous state.

6. Snapshot takes record of whole directories, now just the one you are working on. On the other hand, stage takes the record of your working directory.
