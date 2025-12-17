# GithubCommands-
---------------------Example: Contribute to an existing repository-----------------------------------

# download a repository on GitHub to our machine
# Replace `owner/repo` with the owner and name of the repository to clone
git clone https://github.com/owner/repo.git

# change into the `repo` directory
cd repo

# create a new branch to store any new changes
git branch my-branch

# switch to that branch (line of development)
git checkout my-branch

# make changes, for example, edit `file1.md` and `file2.md` using the text editor

# stage the changed files
git add file1.md file2.md

# take a snapshot of the staging area (anything that's been added)
git commit -m "my snapshot"

# push changes to github
git push --set-upstream origin my-branch

--------------------------------------Example: Start a new repository and publish it to GitHub-------------------------------------

# create a new directory, and initialize it with git-specific functions
git init my-repo

# change into the `my-repo` directory
cd my-repo

# create the first file in the project
touch README.md

# git isn't aware of the file, stage it
git add README.md

# take a snapshot of the staging area
git commit -m "add README to initial commit"

# provide the path for the repository you created on github
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY-NAME.git

# push changes to github
git push --set-upstream origin main


-------------------------------------Example: contribute to an existing branch on GitHub------------------------------------
# change into the `repo` directory
cd repo

# update all remote tracking branches, and the currently checked out branch
git pull

# change into the existing branch called `feature-a`
git checkout feature-a

# make changes, for example, edit `file1.md` using the text editor

# stage the changed file
git add file1.md

# take a snapshot of the staging area
git commit -m "edit file1"

# push changes to github
git push


---------About git push----------
The git push command takes two arguments:

A remote name, for example, origin
A branch name, for example, main
For example:

git push REMOTE-NAME BRANCH-NAME
As an example, you usually run git push origin main to push your local changes to your online repository.

--------------Renaming branches--------------
To rename a branch, you'd use the same git push command, but you would add one more argument: the name of the new branch. For example:

git push REMOTE-NAME LOCAL-BRANCH-NAME:REMOTE-BRANCH-NAME
This pushes the LOCAL-BRANCH-NAME to your REMOTE-NAME, but it is renamed to REMOTE-BRANCH-NAME.

