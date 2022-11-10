# Slab-Session2

After that, we solve problem for inputs at most 10 in branch dev, and we merge this branch into branch main

Now, we improve the code in branch dev and solve problem for inputs at most 30.

Since we have changed both README.md and sum.py, we want to add and commit them separately. First, we add both of them; then, we undo adding README.md by the following command:

git restore --staged README.md

At the end, we commit both changes seperately.

At the same time, in bran dev2, we solve problem for inputs at most 50. This way we will have to solve conflicts at the end.
