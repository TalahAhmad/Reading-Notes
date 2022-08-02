# 03- Revisions and the Cloud

## Version Control

- Allows you to revisit various versions or a set of files by recording changes

- revert a file, track modifications, modify individuals, and comapre changes

### Local Version Control

- entails one database that stores changes to files

### Centralized Version Control

- CVCS: Centralized Version Control System

- a single server stores all changes and file versions; can be accessed by various clients

- streamlined collaboration, knowledge increase on team members activities, and more control to admins

### Distributed Version Control (DVCS)

- addresses the major vulnerability of the CVS: serve as a single point of failure

- if CVS goes down, collabarators cannot work together and save changes to make a new version ; all work will be lost in event of corruption

- DVCS alows clients to create mirrored repos
- programmers collaborate to create simultaneous worl flow

### What is Git?

- a Dvcs that stores data in a system made up of snapshots

- **Snapshots**: each time a changed version of your project is saved is called a *commit*
    git creates a snapshot of the file and stores a reference

- **Local Ops**: most necessary info  can be found in local resources
    allows for process expediency because you aren't online or connected to a VPN, you're on a local disk

- **Tracking changes**: all changes are tracked by Git

- **Loss of Data** Git makes it extremely difficult for you to lose a snapshot of your file

-**States**: files reside in three main states // **committed, modified and staged**
    -comitted: dates is secure in a local database

    -modified: files been changed but not comitted to the database

    -staged: flagged a file's changed version for the next snapshot

## History of Git

- started from a DVCS called BitkEeper in '02

- in '05, Linux and Bitkeeper had tensions so the DVCS was revoked

- Linus Torvals began Git (chief architect of Linux kernal)

-created in '05 is now the most utilized Version Control Systems in the world

## Getting Started

### Download Git

- Git can be installed in three ways:

    Install as a package
    Install via another installer
    Download and compile the source code.

**Mac OS X**

- Terminal: The simplest method for installing Git on a Mac is running Git from the Terminal.

- Git Website

- GitHub: A third option is to install Git as part of the GitHub for Mac install.

### Graphical Clients

- includes GUI (graphic user interface) tools; you can use thrid party tools for specific platforms

### Initial Customization

after installing Git, perform customization steps

- **Configuration of Variables**: "git config" allows the setting of configuration variables that control aspects of Git’s operation and look

- **Identity Setting**: users should immediately set the user name and email address

- **Default Text Editor**: Git will use the system’s default editor; To configure a different text editor // "$ git config --global core.editor emacs"

**Check Settings**: To check settings, use the "git config --list command"

**Getting Help**: three ways to get info on a command //
    "git help command"
    "git command --help"
    "man git-command"

## Setting up a Git Repo

### Importing

Follow these setps:

1. Switch to the target project’s directory

    ex: cd test

2. Use the git init command

    git init

you have created a new subdirectory named .git that has the repository files. Tracking has not commenced

3. To start tracking these repository files, perform an initial commit by typing the following

    git add *.c
    git add LICENSE
    git commit -m “any message here”
Files are now being tracked

### Cloning

- **cloning**: form the cloud (GitHub in this instance) to our local machine (MacBook)
  - Clone that repo
    - click the big green button that says "Code"
    - click HTTPS (for now) and copy that link
    - open your terminal up and navigate to where you want the file to be
    - pwd, ls, cd etc.
    - type **"git clone"** then paste the link
    - click enter
  - to switch from 102 to repo type "cd "file name""
    - now it is switched to git instead of a directory
  - **"git remove -v"** shows you where you are in terminal
  - **"git status"** tells you what's going on
  - "code ."
  
## Workflow

### Local Repo Structure

- Git repo has three components:
    1. After you edit a file, Git flags it as modified because of changes made after the previous commit.
    2. You stage the modified file.
    3. Then, you commit staged changes.

### Check File Status

- utilize the "git status" command

  - add, commit, push
  - **"git add (file name)"** add file to git hub
    - to add multiple files "git add newfile.md newfile2.md" or "git add ."
      - the message will be the same for all the files (-m)
    - staging the picture
  - **"git commit"** commits changes to read.me file
    - **"git commit -m (message)"**
      - annotates and shows on git
      - (-m) adds message
      - if you see "dquote>" your commit and add didn't work
        - ex: added punctuation (. , !)
      - taking the picture
  - **"git push origin main"** (in 102) add it to GitHub
    - PUSHED IT TO THE CLOUD
    - giving the picture to who its going to
  - red= take stuff out
  - green= added new stuff in
- Pulling from GitHub to Terminal
  - always do this process if you make changes on GitHub
  - type **"git pull origin main"**
  - code .

## Stashing Changes

- "git stash": not ready to commit changes but do not want to lose them either

-"git stash apply": When you are ready to continue working on the changes

### Remote Repos

- you can work with multiple repos and each has different privelages

### Cloned Repos

- Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch