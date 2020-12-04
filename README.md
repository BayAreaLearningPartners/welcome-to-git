# Welcome to Git
This is the place where we will gather notes and resources for our upcoming class on December 3, 2020. 

## First steps
Open and tackle the steps in [before-class-homework](/before-class-homework)

## Adding items
If you are a member of the BayAreaLearningPartners organization on GitHub, then you have write access to this repository.  Feel free to add any helpful how-to's or references to this repository as a way to practice working with git. 

## Resources
- [slides from the class](https://docs.google.com/presentation/d/1bobeHLI44tpOqjjM6nmbCGqrDCykj5S21xZR0Rv3ttk/edit?usp=sharing)
- [official git website](https://git-scm.com)  Specifically: [About](https://git-scm.com/about) for overviews [documentation>reference](https://git-scm.com/docs/) for grouped commands

## Glossary
These definitions apply to our specific choice of tools and workflow; they are not the most general definitions.  For example, you could "push" a commit to a repository other than our "blessed repository" on GitHub, but *for us* this is what push means. 

### repository a.k.a. repo
A project that is under version control.  Structurally, this is a folder (a.k.a. directory) that has git superpowers because it has the hidden ".git" folder in it.  Changes made to files in a repository will be noticed by git unless they are set up to be ignored (somehting we didn't cover. search: ".gitignore") 

### commit
A snapshot of your project at a point it time that has a description.  In GitHub Desktop, you create this by gathering a group of changes that you have made since the last commit by reviewing which boxes are checked under "changes" tab, typing out a brief description, and pressing "commit to <branch>".  
  
### push
Copying the commits that you have accumulated on your repository to a repository somewhere else.  

### pull
Copying the commits that have accumulated in a repository somewhere else to our local repository.  

### local
On the computer we're sitting in front of.  Not in the cloud.

### remote
A repository that is not local; it is on a computer somewhere else.  GitHub's copy of our repository is a "remote". 

### origin
The blessed or canonical repository that lives in the cloud.  The authoritative repository. 

### markdown
Think of this as light-weight LaTeX.  You type code, but it shows up all pretty.  If you make a normal text file and change the extension to ".md" or ".markdown" you have created a markdown file, and it will show up all pretty on github.  The file you are reading is a markdown file. 

### branch
A named chain of commits.  Let's backup: when you work on a project, you create a series of commits that go into that project repo's history.  This shows up as chain of commits in chronological order in the history.  At each chain link (commit) we can keep going with the chain (branch) we are already on, or start a different chain (branch).  The tree analogy also works here: any time you add a new commit, you can decide if that new commit grows the trunk or create a new branch that shoots off to the side.  The purpose here is to be able to make any number of commits that drive the project towards a particular purpose before impacting the central, "main" or "trunk" project state.  In our case, we were always commiting to "main".  We did not use branches explicitely.  

### merge
Bring two sets of changes together.  This happens in several situations.  
- Morgan and Sophia are working on the same branch at the same time.  Sophia pushes first, which makes the origin (blessed repository) reflect her changes.  Morgan tries to push but GitHub Desktop tells him his local copy of the repository is out-of-date, he has to pull first because if he doesn't, it is possible that his new changes could overwrite some of Sophia's changes on origin.  So Morgan pulls Sophias changes.  Now Morgan's changes and Sophia's changes are both on Morgan's local repository.  Git on Morgan's computer now tries to put these two sets of changes together to create a snapshot of the project that incorporates both sets of changes.  *this last step is a __merge__*.  If git can do this automatically because Sophia and Morgan didn't change any of the same lines, then Morgan can push the merged result.  Yay.  If Sophia and Morgan did change at least one of the same lines, the merge must be completed with Morgan's manual intervention.  
- Alice is editing several practice tests.  She decides to make a separate commit for each test that she edits to keep the history organized.  She knows that Julian will want to review her edits before releasing the edited tests to students, so she makes a new branch called "edit1" and commits all her edits to that new branch.  When she is done, she tells Julian that the edits are ready for review.  Julian looks at the edits, finds them acceptable, and **merges** Alice's branch back into the *main* branch.  The *main* branch now has all of Alice's edits, but before the merge, the *main* branch had none of Alice's edits.  
