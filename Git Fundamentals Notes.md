# Git Fundamentals Notes

## Git

* Git is a "version control" system. Code is written in a Git repository which 
allows you to quickly restore code (similar to savestates).

* Git has many features to help teams of programmers communicate and write code that doesn't conflict.

#### UI vs. Command Line

* Podcast hosts do most of their work through the command line.

## Git 101

* Git can be a pain to set up.
* "git **init**" to create a repository for your code
  * Creates a hidden .git folder
  * Tracks version history and changes
  * Tracks "origins"
* "git **add**"
  * Many options:
    * "git add -A" adds everything tracked in a repository
    * "git add -p" reviews changes
    * "git add -." adds everything
  * Make a ".git ignore" file
    * None of your files are being tracked initially
    * **_Create the file before doing "git add"_**
    * Ignore lists files you don't want to be part of your repository
* "git **commit**"
  * Writes changes into code
  * Commit message
    * Defines what has happened in the commit
    * Describe the code
    * "git commit -m . . ."
* "git **push**"
  * Git hosts your code on the cloud
  * "git remote add origin . . ."
  * "git push origin . . ."
  * _Origins_ are git respositories that are elsewhere
* "git **pull**" brings down all changes from specified location
* "git **clone**" fetches entire history and repository
* Branches
  * Master changed to Main
  * You can "**checkout**" to main branch and return to your workspace
  * "**merge**" changes into main branch
    * Can get merge conflicts
* "git **fetch**"
  * Gets everything (similar to "git pull")
  * Fetch stages code
* "git **stash**"
  * "Sweeps under the rug" unwanted changes
  * "git stash apply"
* "git **fork**"
  * Not part of Git
  * Creates own version of a repository
  * Fork is entire repository of branches
  * You can make a pull request from your fork to the original project (i.e. suggested changes)
* "git **status**" shows updates
* Merge vs. Pull request
  * Two ways to move code between forks/branches
  * Merge - merges two branches of code
  * Pull - request code to be added
* Git vs. GitHub
  * GitHub hosts your code online
  * GitLab and Bitbucket are alternatives to GitHub
  * Companies may not want their code hosted on a Microsoft-owned service

## Common Issues

* Merge conflicts
* Files tracked unintentionally
  * Hard to get rid of
  * alias git remove ignore (gri)
  * "git rm -r"
* Databases
  * Not compatible with Git

## Git Clients

* Clients add features on top of the command line
* GUIs
* GitHub CLI
* Git Kraken
* GitHub Desktop
* Visual Studio Code extensions