## **GIT BASH COMMANDS**

Git. It is a free and open source distributed version control system(VCS) designed to handle everything

I will give some basic definitions used in git:

Branch: A branch is an independent line of development

Tag: Mark a specific point in time on a branch

Checkout: Get a specific branch to start making your changes 

Commit: Add changes you have made to the repository

Push: Send changes to a remote directory

Workspace: Directory where you store the repository on your computer

Working Area: Files that have been modified but not committed

Staging Area: Modified/added files that are marked to go into the next commit

Local repo: Local copy of the upstream repo

**Basic commands of bash**

`cd NAME-OF-DIRECTORY` Go into a directory to work in it

`cd ..`Go back one directory

`ls`List what is in the current directory

`ls a*`  List what is the the current directory that starts with `a`

`ls *.md`  List what is in the current directory that ends with `.md`

`mkdir NAME-OF-YOUR-DIRECTORY`  Create a new directory

`cat README.md` Display the contents of a text file you created previously

`pwd`  Show the current directory

`clear`  Clear the shell window






**Log in (setting a name and email)**

`git config -global user.name "xxxx"` in xxxx goes your name

`git config -global user.name "emailAdress"`


**Initializate a directory as a git repository**

`git init` Initializate with it

`git clone www.heregoesthelinkoftherepository.com`  Clone the files of a repository


**Add a file to the staging area**

`git add NameOfTheFile`




**Save your changes in the file**

`git commit -m "NameOfChange"` Record your changes permanently

`git commit -a` This command commits any files you have added with the git add command


**See the differences of the not staged files**

`git diff` This command shows the differences which are not yet staged


**Show all the commitments you have done**

`git status` This command lists all the files that have to be commited


**See the version history of the current branch**

`git log`  This command is used to list the version history for the current branch


**Send the committed changes to your remot repository**

`git push` This command sends the committed changes of master branch to your remote repository



