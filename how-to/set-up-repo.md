# Setting Up a Repository

## Create the repo locally 
1. Open Github Desktop
1. File > New repository
1. Choose appropriate name and description
1. (recommended) Choose "Initialize this repository with a README"
1. (recommended) Under "Git ignore" select "Tex"
1. Click "Create Repository"

## Publish your local repo to Github
1. In the Ribbon, click "Publish repository" 
1. Does this belong in the balp organization?  

## Adjust your .gitignore
1. Decide which files and folders you want to ignore
1. Add pattern that matches those files. 
1. Add exceptions. 
1. Save .gitignore - changes should disappear in sidebar
1. Commit your changes to .gitignore. 

## Include latex-library as a submodule
1. In menubar click Repository > Open in Git Bash  or Open in Terminal
1. In your browser, grab the URL of the latex-library (copy to clipboard)
1. In the terminal run: `git submodule add -b main https://github.com/BayAreaLearningPartners/latex-library.git`
1. Commit your changes

# Working with your Repo
## Updating latex-library
If there are updates in the main branch of latex-library that you want to include in your repo, you need to explicitly tell your repo to go get the latest version of latex-library.  
1. With your repo open in your terminal, run: 

    `git submodule update --remote`
1. Commit and push this update so it will propagate to your collaborators. 

## Adding Collaborators
Because we did not put the repo in the BALP organization on github, you determine who has access on github.  In your repo's home page on Github, under "settings" see the "Manage access" button on the left navbar.  This is where you get to be the bouncer.  

# Notes about the terminal
## Typing things in
- There are special key-bindings for copy/paste.  Ctrl-C, Ctrl-V don't work.  
- What's worse, Ctrl-V can produce a hidden character which will mess up the command, but it will look right.  I know!!!  
- When you enter a password in the terminal, you won't see any characters. 

## Commands
- When a dash `-` precedes a character, or two dashes `--` precede a kebab-case word or phrase, these are options sent to the command. Many options have both a shorthand version with a dash and a single character and a longhand version with two dashes and a more self-explanatory phrase, and both will do the same thing. 
- To check whether a program is installed, or see what version is installed, use the `--version` option. E.g. `git --version` or `tlmgr --version`
- To see help, use `--help` 