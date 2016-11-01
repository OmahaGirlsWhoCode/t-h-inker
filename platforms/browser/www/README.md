#Git Practice

You will be practicing git commands and how you should use git to work on a project.





#Glossary

The commands you will learn today are:


 - git clone

`git clone git@github.com:username/some_repository_name.git`

This command allows you to copy a repository that you already have on GitHub and copy it locally.


 - git status

`git status`

This command allows you to see the status of your local files and whether they have changed or are staged for a commit.


 - git add

 `git add .` or `git add file.js`

 This command will allow you to stage the changes to all files, so that they are _ready_ to commit.  It will not commit any files.


 - git commit

`git commit -m "Centers heading 1 text"

This command will _commit_ the changes you have made.  It will create a _commit message_ that says 'Centers heading 1 text', so that people can see what you were doing.  


 - get checkout

 `git checkout -b newBranch` to create a new branch or `git checkout newBranch` if it already exists.

 Master is the default branch.  But you should create and work on new branches, so that you don't inject code that is not tested into Master for other people.  Each person works on a branch.  Then you merge your branch into master when your code is tested and ready.


  - git pull

 `git pull origin branch_name`

Before you do a merge, you should pull down changes from GitHub to make sure you aren't missing any changes.  You must _pull_ before you _push_.


  - git merge

`git merge newBranch master` when you are merging master _into_ your branch (newBranch is checked out).
`git merge master newBranch` when you are _closing_ your branch (master is checked out).

  - git push

`git push origin branch_name`


