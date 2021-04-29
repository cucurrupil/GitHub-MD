###### **GIT BASH COMMANDS**

Git. It is a free and open source distributed version control system(VCS) designed to handle everything

I will give some basic definitions used in git:

**Branch**: A branch is an independent line of development

**Tag**: Mark a specific point in time on a branch

**Checkout**: Get a specific branch to start making your changes 

**Commit**: Add changes you have made to the repository

**Push**: Send changes to a remote directory

**Workspace**: Directory where you store the repository on your computer

**Working Area**: Files that have been modified but not committed

**Staging Area**: Modified/added files that are marked to go into the next commit

**Local repo**: Local copy of the upstream repo
  
  
  
  
  

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

`git reset [file]`  --> Revert your **repository** to a previous know working state

`git commit`  --> Create a new **commit** from changes added to the **staging area**.  
The **commit** must have a message

`git rm [file]`  --> Remove file from *working directory* and **staging area**

`git stash`  --> Put current changes in your *working directory* into *stash* for later use

`git stash pop`  --> Apply stored **stash** from all your previous *stashes*

`git stash drop`  --> Delete a specific **stash** from all your previous *stashes*

  
  
  
  
  
**Git branching model**

`git branch [-a]`  --> List all local branches in repository. With -a: show all branches (with remote)

`git branch [branchName]`  --> Create a new branch, referencing the current *HEAD*

`git checkout [-b][branchName]`  --> Switch *working directory* to the specified branch. With -b

`git merge [fromName]`  --> Join specified fromName branch into your current branch (the one you are on currently)

`git branch -d [name]`  --> Remove selected branch, if it is already merged into any other.  
*-D* instead of *-d* forces deletion


**Review your work**
  
  
  
  
  
`git log [-n count]`  --> List commit history of current branch, **-n count** limits list to last **n** commits

`git log --oneline --graph -- decorate`  --> An overview with reference labels and history graph. One commit per line

`git log ref..`  --> List commits that are prensent on the current branch and not merged into **ref** . A **ref** can be a branch name or a tag name

`git log ..ref`  --> List commit that are present on **ref** and not merged into current branch

`git reflog` --> List operations (like checkouts or commits) made on local repository
  
  
  
  
  
**Tagging known commits**

`git tag`  --> List all tags

`git tag [name] [commit sha]`  --> Create a tag reference named **name** for current commit. Add **commit sha** to tag a specific commit instead of current one

`git tag -a [name] [commit sha]`  --> Create a tag object named **name** for current commit

`git tag -d [name]`  --> Remove a tag from local repository
  
  
  
  
  
**Reverting changes**

`git reset [--hard] [target reference]`  --> Switches the current branch to the **target reference,** leaving a difference as an uncommitted change. When **--hard** is used, all changes are discarded

`git revert [commit sha]`  --> Create a new commit, reverting changes from the specified commit. It generates an **inversion** of changes

  
  
  
  
  
**Synchronizing repositories**

`git fetch [remote]`  --> Fetch changes from the **remote,** but not update tracking branches

`git fetch --prune [remote]`  --> Delete remote Refs that were removed from the **remote** repository

`git pull [remote]`  --> Fetch changes from the **remote** and merge current branch with its upstream

`git push [--tags] [remote]`  --> Push local changes to the **remote.** Use **tags** to push tags

`git push -u [remote] [branch]`  --> Push local branch to **remote** repository. Set its copy as an upstream


**Another useful commands**


`-rm -rf fileName`  --> Delete directories

`../`  --> Go up one folder

`find .-name "\*.txt"`  --> Used to find files (with any name) with a specific file format

`-grep "wordToFind" fileWhereYouAreSearching.txt`  --> Look for a specific word into a file

`wc fileName.txt`  --> Show number of words, bytes and lines of such file

`nano fileName.md`  --> Nano open the text editor. If **fileName.md** is included the text editor will open the new file with that name and file format







