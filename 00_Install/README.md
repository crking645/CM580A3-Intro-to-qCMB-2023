# Setup Installation Basics

There are a few Apps that we want to have in hand as we get started. They are Github Desktop and R/RStudio.  As we use the command line, there will be other components to install and get working, but that will come later.

## Your username and password

I know this seems silly, but make sure you have your login username and password for your computer- you may already use it regularly to login. You'll need it to install things.  You may wish to write it down somewhere.

If you are able to install things already, then you're all set to go!

## Installing on Mac versus Windows

Mac install files are disk images that end in the file extension ".dmg". Windows install files might end in ".exe" (I don't have Windows), but you may have to install through the Start Menu for the Windows "allowed" version.

## Github desktop to access course content

### Github account

It may go smoother if you have a github account. Sign up at github.com

### Github Desktop Download

https://desktop.github.com/ Should detect your necessary version. Click to download.

You can log in with your account once you've downloaded the App.

Windows users will need to install git. Download from https://git-scm.com/

### Cloning the course repository

* Under Current Repository, click the down arrow -> Add -> Clone 
* Find the URL tab, and paste in https://github.com/Colorado-State-University-CMB/CM580A3-Intro-to-qCMB-2023.git
* It will ask you where on your computer you want to put it, so have a place in mind for the coursework.
* Click "clone" once you are done.
* You will see the files in the right pane when the repository is loaded/selected. You can view them on your computer with 
  * Mac: "Show in Finder"
  * Windows: "Show in Explorer"

We will go through an exercise on how to load and refresh course content.

## R

Current version is 4.2.2. I'm using 4.1.2. 

If you already have R, but a previous version, it should work for most things but you can update using the same instructions as below. You may have to reinstall packages if you do this though.


Go to: https://cran.rstudio.com/ 

* Windows: 
  * Click "Download R for Windows"
  * You need "base" and "Rtools"
  * Download the ".exe" file and click on it
  
* Mac:
  * Click "Download R for Mac"
  * You need to know if you have an Intel or Apple Silicon processor
    * Click on the Apple symbol at the very top left of your screen. Choose "About this Mac"
    * Under "Processor" look for the words "Intel" or "Apple Silicon." There will be other details but these words are the important ones.
  * If you have intel: Download "R-4.2.2.pkg (notarized and signed" and click on it to install.
  * If you have Apple Silicon: Download "R-4.2.2-arm64.pkg (notarized and signed)" and click on it to install.


## RStudio

https://posit.co/download/rstudio-desktop/#download

* Windows installer ends with *.exe*
* Mac installer ends with *.dmg*

## Swirl

Swirl is a package that runs in RStudio to provide extra instruction. It is good to have this installed.

Find your RStudio console to type in the following commands. [How to find the console.](https://www.google.com/search?q=rstudio+where+is+the+console&oq=rstudio+where+is+the+console)

Type the following into the console and hit return:
```r
install.packages("swirl")
```

Check the installation by typing the following into the console and hitting return.
```r
library("swirl")
```


## For Dr. Brooke Anderson's Module (Feb 20th): Tex software for creating PDF documents.

### Mac

Download and install MacText from https://tug.org/mactex/

This was very large when I downloaded it: 7GB!


### Windows

Download and install MiKTeX from http://miktex.org


## Get ahead of things by installing a few R libraries

Just be on the look out for ERRORS (tend to be red).

```r
install.packages("tidyverse")
library(tidyverse)
```

```r
install.packages("BiocManager")
library(BiocManager)
```

To install from Bioconductor, we use a slightly different install command.

```r
BiocManager::install("biomaRt")
library(biomaRt)
```


