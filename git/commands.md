# Git guide

# What is git used for?
1. Track changes in files.
2. Compare project versions.
3. Rollback to earlier versions.
4. Collaborate and share changes.
5. Merge changes.

# Git & GitHub
* **Git**
  * Version Control System.
  * Local PC.
  * Push repository to GitHub.
* **GitHub**
  * Online.
  * Stores repositories on a server.
  * Team collaboration with git repositories.

# What is ...
* **GitHub forks**
  * Only exist in GitHub.
  * Option to clone a repo to your GitHub account, so you can access.
* **branch**
  * It's a copy of the project.
* **.gitignore. -** file where files can be ignored. It is in the root of the repo.

# Git stages.
1. **Working Directory**
    * Where we are working.
2. **Staging area**
    * Where worked files are addded before doing a commit.
3. **Repository**
    * Where worked files are after doing a commit.
4. **Work > stage > repository**
5. **Work > git add > git commit**

# Basic commands to use the console.
* **start .**
  * Opens windows file explorer
 
# Git initial configuration
* **git config --global user.name "Name Lastname"**
  * User name globally.
  * Identify who is making a commit.
* **git config --global user.name "Name Lastname"**
  * User email globally.
* **git config user.name**
  * Displays the configured username.
* **git config user.email**
  * Displays the configured email.
* **git config --global core.editor "code --wait"**
  * Sets by default visual studio code as text editor.
* **--global**
  * Sets the global configuration.
  * Remove if different configurations are required.
     
# Git commands
*  **git init**
  * Initialize a git repository
* **git add fileName**
  * Adds the file/files to staging area.
* **git add .**
  * Adds modified files to staging area.
* **git commit**
  * Commits changes with a large message (opens in editor).
* **git commit -m "message"**
  * Commits all changes from the staging area.
  * Must have a comment to identify the changes.
  * Opens text editor to write big comments.
* **git commit -a -m "comment"**
  * Commits the changes directly.
  * -a. - adds the file to staging area
*  **git diff fileName**
   * Compare changes in the file.
* **git diff commitId**
  * Shows the difference between actual work and referenced commitId (e54a1b6).
 * **git diff commitId commitId**
  * Shows the differences between these two commits.
 * **git diff HEAD~X HEAD~X**
  * Shows the differences between these two commits X commits ago before HEAD/MASTER.
* **git status**
  * Shows the status of the actual work.
  * If we want changes from remote repo, execute git fetch.
* **git log**
  * Shows previous commits made by users.
* **git show commitId**
  * Shows detailed information of the commit.
* **git show HEAD~X**
  * Shows detailed information of the commit X commits ago before HEAD/master.
* **git annotate fileName**
  * Shows the logs related to this file.
* **git checkout --fileName**
  * Revert changes and back to original version before modifications.
* **git checkout .**
  * Revert changes to files and back them to original version before modifications.
* **git checkout commitId fileName**
  * Revert changes and back to commitId version evend when pushed to remote repo.
* **git reset HEAD --fileName**
  * Unstages changes when are staged.
* **git reset HEAD .**
  * Unstages all changes when are staged.
* **git branch**
  * Lists of all created branches.
* **git branch branchName**
  * Creates a new branch.
* **git checkout branchName**
  * Switch to a branch.
* **git checkout -b branchName**
  * Creates and switches to a branch.
* **.gitignore**
  * .dll - will ignore .dll files
  * folderName/ - will ignore an entire folder.
  * folderName/*.txt - will ignore .txt files inse a folder.
  * *.log - will ignore any files with the .log extension.
  * Ignore will only work when files is not in repository.
  * If file is already in repository, it has to be deleted.

   
# Remote repositories
* **git remote add remoteName repositoryUrl**
  * Add GitHub repository to local PC.
  * remoteName. - origin (common name)
  * repsitoryUrl. - https://github.com/abelgmz/GitCourses.git
* **git pull remoteName branchName**
  * Gets last version of the branch from GitHub.
  * remoteName. - origin (common name).
  * branch. - master.
* **git branch --set-upstream-to=origin/master master**
  * Local branch will be tracking remote branch for new changes.
* **git pull**
  * Gets last version of the branch from GitHub directly.
* **git fetch**
  * Downloads all changes from remote repo.
  * Files are not shown as available, just aware of their existance.
* **git clone repositoryUrl**
  * Clones a remote repository.
  * Create new folder where the repo will be downloaded.
