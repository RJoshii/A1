
Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (master)
$ git init
Reinitialized existing Git repository in C:/Users/Rashmi Joshi/Desktop/git/.git/

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (master)
$ git add sample.txt

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (master)
$ git commit -m "Add sample.txt file"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Rashmi Joshi@DESKTOP-IEQGFKR.(none)')

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (master)
$ git config --global user.email "rashmijoshi873@gmail.com"

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (master)
$ ^C

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (master)
$ git config --global user.name "RJoshii"

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (master)
$ git commit -m "Add sample.txt file"
[master (root-commit) b5d9b97] Add sample.txt file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 sample.txt

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (master)
$ git checkout -b feature-branch
Switched to a new branch 'feature-branch'

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (feature-branch)
$ git add sample.txt

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (feature-branch)
$ git commit -m "Add new content to sample.txt file"
[feature-branch 211d34b] Add new content to sample.txt file
 1 file changed, 1 insertion(+)

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (feature-branch)
$ git checkout master
Switched to branch 'master'

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (master)
$ git merge feature-branch
Updating b5d9b97..211d34b
Fast-forward
 sample.txt | 1 +
 1 file changed, 1 insertion(+)

Rashmi Joshi@DESKTOP-IEQGFKR MINGW64 ~/Desktop/git (master)

**Explanation**
Step-by-step instructions to initialize a local git repository in a new directory and add a text file named "sample.txt" to the repository, commit the file with a meaningful message, create a new branch called "feature-branch" and switch to that branch, add some content to "sample.txt" and commit the changes, and merge the "feature-branch" back into the main branch (usually "master" or "main"), resolving any conflicts if they occur:
To initialize a local git repository in a new directory:
1.	Open Terminal.
2.	Navigate to the directory where you want to create the new repository.
3.	Run the following command:

git init


This will create a new .git directory in the current directory, which will contain all of the repository's metadata.
To add a text file named "sample.txt" to the repository:
1.	Create a new text file named sample.txt.
2.	Open the file and add some content.
3.	Save the file.
4.	Run the following command to add the file to the staging area:

git add sample.txt


To commit the file with a meaningful message:
1.	Run the following command to commit the changes:

git commit -m "Add sample.txt file"


The -m flag allows you to specify a commit message.
To create a new branch called "feature-branch" and switch to that branch:
1.	Run the following command to create the new branch:

git checkout -b feature-branch


This will create a new branch called feature-branch and switch to it.
To add some content to "sample.txt" and commit the changes:
1.	Open the sample.txt file and add some new content.
2.	Save the file.
3.	Run the following command to add the changes to the staging area:

git add sample.txt


4.	Run the following command to commit the changes:

git commit -m "Add new content to sample.txt file"


To merge the "feature-branch" back into the main branch (usually "master" or "main"), resolving any conflicts if they occur:
1.	Switch back to the main branch:

git checkout main


2.	Run the following command to merge the feature-branch into the main branch:

git merge feature-branch


If there are any conflicts, Git will prompt you to resolve them. Once you have resolved all of the conflicts, commit the changes.
Here is an example of a complete workflow:

# Initialize a local git repository in a new directory
git init

# Add a text file named "sample.txt" to the repository
echo "This is the initial content of sample.txt" > sample.txt
git add sample.txt
git commit -m "Add sample.txt file"

# Create a new branch called "feature-branch" and switch to that branch
git checkout -b feature-branch

# Add some new content to "sample.txt" and commit the changes
echo "This is the new content of sample.txt" >> sample.txt
git add sample.txt
git commit -m "Add new content to sample.txt file"

# Switch back to the main branch
git checkout main

# Merge the "feature-branch" back into the main branch
git merge feature-branch


If you encounter any conflicts while merging the branches, you can resolve them manually or use a tool like GitKraken to help you.

