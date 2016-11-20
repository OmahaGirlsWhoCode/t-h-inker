#T(h)inker

This is the repo for Omaha Girls Who Code high school class, Session 2 project.

T(h)inker is an app for users who have anxiety or ADD..

#Coding
The complete configuration file is needed to create a cordova app.  HTML, CSS, and JS files should go inside the www folder.

Clone this repository into cloud9.

Make sure you work off of branches.

#Git Review
#Example Workflow

1. Clone a repository

	`git clone git@github.com:username/some_repository_name.git`

2. Create and checkout a branch

	`git checkout -b myBranch`

3. Make a change and save it.

4. Add the changed files to the staging table.

	`git add .`

5. Commit the change.

	`git commit -m "Made my first change"`

6. Repeat steps 4-5 until your a small day's work is done and tested.

7. Pull down changes from GitHub in case your team has made changes since you started working.

	`git pull origin master`

8. Merge your branch with any changes you pulled down from the master branch.

	`git merge myBranch master`

9. Checkout master.

	`git checkout master`

10. Merge master with your branch to close your branch.

	`git merge master myBranch`

11. Push your changes so that others can see them.

	```
	git push origin master
	git push origin myBranch
	```


#Use Cloud9 to develop the app


Cloud9 offers workspaces that are like virtual machines (virtual computers) with all the right software installed.

In this case, we need git, HTML5, and a server we can use to render the HTML/CSS/JavaScript.

You should have been invited by email to use a student account.  

1. Log into or set up your Clouod9 account.  
2. Make sure your CLoud9 account is connected to your GitHub account.
3. On GitHub, click 'Clone or Download' and copy the SSH (not HTTPS) url to this repo.
4. On Cloud9, create a new workspace using this SSH url and set up a HTML workspace.
5. Open the workspace.



#Build the Mobile App using PhoneGap Build

##Setting Up the App
This repository was made using the template app from cordova.  To find out more check out the [cordova documentation](https://cordova.apache.org/docs/en/latest/guide/cli/).

`cordova create appName`


The `config.xml` file was updated for this file.

 - the widget xml has the id of the app, the version, the website
 - name of the app
 - description of the app
 - author and author website (omahagirlswhocode)
 - content source lists the file that should open when the app opens (www/index.html)

A few plugins were installed:
 - cordova-plugin-whitelist to keep the app secure and not allow css or JS from other sources to load
 - cordova-plugin-splashcreen that allows a splash icon to appear while the app is loading
 - cordova-plugin-vibration allows vibration

All the HTML, CSS, and JS are in the www folder.  The splash icons are in the res folder.  The other folders are needed to build the app but should not normally be modified.


##Testing the app
If phonegap is installed, you can run `phonegap serve` to run a phonegap server and test it on [http://emulate.phonegap.com/](http://emulate.phonegap.com/).


##Devloper license
Google requires a Google Play Developer account, and then you can publish an app on Google Play Developer Console.  Check out the documentation [here](https://support.google.com/googleplay/android-developer/answer/6112435?visit_id=1-636151849476603622-1643489180&rd=1).  Once you have created an app, you can get the license key.


##Building the app

Use [PhoneGap Build's online tool](https://build.phonegap.com/apps) to build the app (.sdk).  Add the license key.




#Git Glossary

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

	`git commit -m "Centers heading 1 text"`

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
