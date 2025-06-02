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

---------------------------------------------------------------------------------------------------------
register https://github.com
install git bash @https://git-scm.com/downloads

-----------------------------------------------------------------------------------------------------------
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

