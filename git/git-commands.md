# Working with Git commands

### Installation

To start working with Git commands you first need to install and setup Git in your machine. Follow the instructions here https://github.com/git-guides/install-git

Sync your GitHub account with VSCode by signing in from the bottom left in the VSCode menu "Accounts".

### Using VSCode GUI

You can use the graphical user interface of your Visual Studio Code editor to run Git operations.

To stage your changes:
- Go to the 'Source Control' tab on the left menu in VSCode. You will see all your staged and unstaged files.
![Alt text](/images/git-gui-stage.png "Stage changes")
- Select all the files to be pushed and click on any of the + signs 
- Put in a message and click on "Commit"
- Then on the bottom of your editor, you will see a refresh symbol with one change to push. Click on that button and your changes will be pushed to github.

### Using VSCode terminal

To use the terminal in VSCode, go to "Terminal" in the top and click on "New Terminal"

- git config: This command sets the author name and email address respectively to be used with your commits.
![Alt text](/images/git-config.png "Git Config")
- git init: This command is used to start a new repository.
![Alt text](/images/git-init.png "Git Init")
- git clone: This command is used to obtain a repository from an existing URL. You can either use HTTPS or SSH to clone. If you wish to use SSH then you need to create an SSH key in your github account.
![Alt text](/images/git-clone.png "Git Clone")
- git add
    - git add [file]: This command adds a file to the staging area.
    - git add * OR git add .: This command adds one or more to the staging area.
- git commit: This command records or snapshots the file permanently in the version history.
![Alt text](/images/git-commit.png "Git Commit")
- git diff: This command shows the file differences which are not yet staged. (Press Q to exit)
- git status: This command lists all the files that have to be committed.
![Alt text](/images/git-status.png "Git Status")
- git branch: This command lists all the local branches in the current repository. (Press Q to exit)
![Alt text](/images/git-branch.png "Git Branch")