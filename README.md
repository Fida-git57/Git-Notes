# Git-Notes
Git is a version control system used for tracking changes in computer files. 
It is generally used for source code management in software development

Git is a version control system used for tracking changes in computer files. It is generally used for 
source code management in software development

------------------------------------------------------------------------------------------------------------------------------
Features of Git 
	Tracks history
	Free and open source
	Supports non-linear development 
	Creates backups
	Scalable
 	Supports collaboration 
	Branching is easier 
	Distributed development

----------------------------------------------------------------------------------------------------------------
What is the difference between git and GitHub?
	While Git is a tool that's used to manage multiple versions of source code edits that are then 
transferred to files in a Git repository
	GitHub serves as a location for uploading copies of a Git repository.

1., Git is a software., GitHub is a service.
2., Git is a command-line tool, GitHub is a graphical user interface 
3., Git is installed locally on the system, GitHub is hosted on the web 
4., Git is maintained by linux., GitHub is maintained by Microsoft.
5., Git is focused on version control and code sharing., GitHub is focused on centralized source code hosting.
6., Git is a version control system to manage source code history.
 GitHub is a hosting service for Git repositories.
7., Git has no user management feature.
 , GitHub has a built-in user management feature.
8., Git is open-source licensed., GitHub includes a free-tier and pay-for-use tier.
9., Git has minimal external tool configuration., GitHub has an active marketplace for tool integration.

What is Version Control System?
When developers are creating something (an application, for example), they are making constant changes to the code and releasing new versions, up to and after the first official (non-beta) release.

------------------------------------------------------------------------------------------------
register https://github.com
install git bash @https://git-scm.com/downloads

------------------------------------------------------------------------------------------------
Git Commands
--------------
cd Desktop

git init --> create the empty local repositry
Then it will create 3 logical areas

working area 			staging area						loacl repositry		     Remote repo
-------------			-------------						----------------	     ------------
vi DBUtils.java			it is a area which
--This file will be 	 	is intermetent b/w 
in working area			working and local 
				which contains the file

61git status -->where the files are available-->working,staging,local area

To move files from working area to staging area
---> git add .
	 git add *
	 git add *.java --> to move all the java files
	 git add DBUtilis.java --> to move inly 1 file

 when will we move files from working area to staging area
	Once development is complete will move the files from working area to the staging area

git commit -m "First commit" --> To commit the file from staging to local repositry
	m=message
 git commit -a -m "Updated"
	a=changing area

 ----------------------------------------------------------------------------------------------
When you install Git-bash, the first thing you should be doing is setting up your user details as follows only one time.

#git config --global user.name "Fida Learning " 
#git config --global user.email "fidaarooj57@gmail.com"

Checking for settings 
#git config –list
#git config --global--list --> to see if we have configured correct username and email.if

#git config --global --edit

You can also check what Git thinks a specific key’s value is by typing git config <key>:
#git config user.name

The files which are available in working area are untraked files display in red colour
The files which are availabe in staging area are tracked files and display in green colour

----------------------------------------------------------------------------------------------
Task 1: Start a new repository and publish it to GitHub
-----------------------------------------------------------------------------------------
Go to the directory where you want to create the git repository. 

#cd ~/Desktop
#mkdir git-practice-commands 
#cd git-practice-commands

#git init : Create a local Git empty repository.
Initialized empty Git repository in /Users/Fidaarooj/git/git-practice-commands/.git/
#git status : Gives the status of your untracked files. 
#touch DBConnect.java
#git status
#vim DBConnect.java
#git add DBConnect.java: Add the files(here DBConnect.java) into your staging area. 
#git status
On branch master 

Initial commit

Changes to be committed:
(use "git rm --cached <file>..." to unstage) 

------------------------------------------------------------------------------------------------
IDEs--> Integrated Development Environment

Java IDEs--> Eclipse
			 MyEclipse
			 Intellij
			 
git add .
git add *
git add 

git remote add aliasname remote repo url : Adding the URL for the remote repository where your 
local repository code will be pushed.

git remote add cb <link>
	git remote add cb https://github.com/devops-training-sec/citibank.git

git remote -v    --> to check push, fetch

git push aliasname branchname --> the files which are in local repo moves to remote repo
	While using git push command it will ask credentials related to github

#git log : It will give all commit ids.
#git log -2 : It will display only 2 commit ids.

#git show --pretty="" --name-only << Commit ID >> : It will display all the files which are committed in that particular commit.

#git clean -n : It will preview the changes.

#git clean -f : If we want to remove new files from working area.

#git reset <<File Name>> : To untrack the tracked files (revert back to working area from staging area.).

#git revert <<Commit ID>> : It will revert the changes committed in that particular commit id from local repo.

#git push origin master -f: It will revert the changes from remote repo.

----------------------------------------------------------------------------------------------
PAT--> Personal Access Token --> Its like a password to move file from local to remote repo
	
	ghp --> GitHub Public
	ghe --> GitHub Enterprise

------------------------------------------------------------------------------------------------

