# Setting up LaTeX building locally
This guide documents one local setup for coding effectively in LaTeX on your computer.  We are doing this because Overleaf does not support git branches, which essentially prevents any substantially collaborative workflow using git and Overleaf together.  

By doing this, you gain essential tools like branching, and also extremely convenient tools like seeing changes (both yours and others') at a glance.  

## Install TexLive
Click the following link: [install-tl-windows.exe](http://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe) 
This will download the TeX Live installer. 

Run this file when it's done downloading, select "Install" and click "Next", then click "Install"

When you get to an options page, click "Advanced"

Under the Selections category, change the scheme setting from "full scheme (everything)" to "basic scheme (plain and latex)"

Click "Install" and let the installation proceed!

More information about this install lives here: https://www.tug.org/texlive/acquire-netinstall.html

## Install necessary LaTeX Packages
LaTeX compilation depends on a core program (TexLive) and many packages that you add onto that core program that extend the features of the core program.  We chose a basic installation when we installed TeX Live because more thorough installations can take several hours downloading and installing packages you'll never need.  That decision means we don't have many of the packages we'll need.  To install these, it is a matter of running `tlmgr install <package-name>` a bunch.  Fortunately for you, Mike has compiled a list of the packages we use and all you have to do is:
1. Open a terminal
1. copy the following line into your terminal and press enter.
```
tlmgr install latexmk exam subfiles xlop xstring cancel xcolor pgf pgfplots framed amsmath multirow relsize halloweenmath bbding txfonts adjustbox standalone enumitem tabto-ltx titlesec tcolorbox pict2e xkeyval collectbox currfile filehook filemod gincltex svn-prov environ etoolbox pgf-blur collection-fontsrecommended lineno parskip scsnowman
```

## Install VSCode
Visual Studio Code is a code editor that comes with a bunch of functionality built-in, is relatively lightweight, and has a big community maintaining it.  You are, of course, welcome to use a different editor, and the attendant different extensions for working efficiently with LaTeX. 

[Download](https://code.visualstudio.com/download) and install for your OS. 

## Install LaTeX Workshop extension in VSCode
Launch VSCode and click on the "Extensions" tab in the left sidebar menu (should be the bottom one).  In the "Search Extensions in Marketplace" search bar, enter the following: 
`Latex workshop`

Click on the entry called "LaTeX Workshop" (Author: James Yu)

This will bring up the page for this extension to the right.  Click "Install" under the title.  

Because we have already installed TeXLive and all the dependencies for our documents, you should be able to build documents now.  
