###### **GIT BASH COMMANDS**

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

**Basic git workflow with gitlab**

Provides a central repository. You use git locally on your own system to create and update code, share your changes with your team, and see your team's changes by using git commands to push, fetch, and merge work.



`cd NAME-OF-DIRECTORY` --> Go into a directory to work in it

`cd ..`  --> Go back one directory

`ls`  --> List what is in the current directory

`ls a*`  --> List what is the the current directory that starts with `a`

`ls *.md`  --> List what is in the current directory that ends with `.md`

`mkdir NAME-OF-YOUR-DIRECTORY` --> Create a new directory

`cat README.md`  --> Display the contents of a text file you created previously

`pwd`  --> Show the current directory

`clear`  --> Clear the shell window







**Git configuration**

`git config -global user.name "xxxx"` --> Into xxxx goes your name

`git config -global user.name "emailAddress"`  -->Into emailAddress goes your email


**Starting a project**

`git init [projectName]`  --> Create a new repository, if projectName is provided, Git will create a new directory name and will initialize a repository inside it. If the project name is not provided, then a new repository is initialized in the current directory

`git clone [project url]`  --> Download a project with the entire history from the remote repository.


**Daily life commands**

`git status`  --> Display the status of your working directory. Options include new, staged, and modified files. It will retrieve branch name, current commit identifier, and changes pending commit.

`git add [file]`  --> Add a file to the *staging* area. Use in place of the full file path to add all changed files from the *current directory* down into the *directory tree*

`git diff [file]` --> Show changes between *working directory* and *staging area*

`git diff --staged [file]`  --> Shows any change between the *staging area*and the *repository*

`git checkout -- [file]`  --> Discard changes in *working directory*. This operation is *unrecoverable*

`git reset [file]`  --> Revert your *repository* to a previous know working state

`git commit`  --> Create a new *commit* from changes added to the *staging area*.  
The *commit* must have a message

`git rm [file]`  --> Remove file from *working directory* and *staging area*

`git stash`  --> Put current changes in your *working directory* into *stash* for later use

`git stash pop`  --> Apply stored *stash* from all your previous *stashes*

`git stash drop`  --> Delete a specific *stash* from all your previous *stashes*


**Git branching model**

`git branch [-a]`  --> List all local branches in repository. With -a: show all branches (with remote)

`git branch [branchName]`  --> Create a new branch, referencing the current *HEAD*

`git checkout [-b][branchName]`  --> Switch *working directory* to the specified branch. With -b

`git merge [fromName]`  --> Join specified fromName branch into your current branch (the one you are on currently)

`git branch -d [name]`  --> Remove selected branch, if it is already merged into any other.  
*-D* instead of *-d* forces deletion


**Review your work**



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



