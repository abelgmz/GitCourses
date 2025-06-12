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
* **git commit**
  * Commit changes witha a large message (opens in editor).
* **git commit -m "message"**
  * Commits all changes from the staging area.
  * Must have a comment to identify the changes.
  * Opens text editor to write big comments.
*  **git diff fileName**
   * Compare changes in the file.
* **git diff commitId**
  * Shows the difference between actual work and referenced commitId (e54a1b6).
*
