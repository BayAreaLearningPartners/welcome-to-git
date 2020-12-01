# Pre-class assignment
The world of git and GitHub comprises much material, so we all need to have our computers ready before class.  You will be installing two programs: git and gitHub-desktop, which have an overlapping purpose but vastly different user-experience philosophies.  I am exposing you to both because one is a good gateway and the other is how things are done by the pros.  When I began using git, I used both for a while, but today I exclusively use git (when I am not teaching a class on git).  

Just a bit of nomenclature to start.  
**Git** is a *command-line program* that runs on your computer that you will use to manage changes to your documents.  
**GitHub** is a *web service company* and also the web service that company provides (think Google).  
**GitHub-Desktop** is a graphical program that GitHub (the company) provides to make Git (the command-line program) more accessible to learn.  

## Sign up on GitHub
If you have not created an account on github.com (the site you are visiting right now) then click "Sign up" in the upper right.

## Install Git
If you rock a mac, you may already have git installed.  For mac users: open a terminal (press command-space and type "terminal" then run the top result).  Then type `git --version` into the terminal window and press enter.  If you see a version number reported, you already have git and can continue with Install GitHub Desktop.  If you see "command not found" or some such, keep going on the next line.  

Windows users, start here.  
- Navigate to https://git-scm.com/downloads
- Select your operating system to download the program. 
- Once downloaded, run the program
- You can customize your install or select defaults as you see fit with the following constraints:  
  - Under "Select Components": do not uncheck "Select Git LFS (Large File Support)".
  - Under "Choosing the default editor used by Git": Either choose "Use the Nano editor by default" or an editor you already have installed.  Do not choose Vim unless you already are familiar with it. 
  - Under "Adjusting the name of the initial branch in new repositories" select "Override the default branch name" and use "main". 
  - Under "Adjusting your PATH environment" choose "Git from the command line and also from 3rd-party software."
  - Under "Choosing HTTPS transport backend" choose "Use the OpenSSL library"
  - The remaining options should be left as defaults. 

## Install GitHub Desktop
Unless you installed this before, you won't have this on your system.  
- Navigate to https://desktop.github.com
- Download and install for your operating system

You will be asked to provide your github account information.  Please make sure you use the email that you used when signing up for GitHub.  

## Prepare your workspace directory
You will need to pick a folder for your repositories.  A repository is just a folder on your computer that git monitors.  I recommend creating a new folder to keeping all your repositories together.  Personally, I use D:/repos/ (on Windows) /home/repos/ on Linux because I prefer a short path and I like seeing all my repositories in one place.  You may alternatively scatter your repositories out into topic-related folders, for example one repository in a BALP folder, another in the folder where you're writing a novel, but there is one hard requirement: **a repository must not be in a cloud-synced folder.** That means it can not be inside a google drive or a dropbox folder. 

## Video Introduction
Watch the first video [here](https://git-scm.com/videos).   And write down any questions.  Feel free to watch the other 3 videos too, but the first video is the essential one. 
