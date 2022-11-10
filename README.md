# Slab-Session2

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

Finally, we solve problem completely in branch dev by removing if; and we merge it into main using a pull request.

# Questions
