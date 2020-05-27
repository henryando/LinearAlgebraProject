# Linear Algebra for Data Science

## Overview

We are developing a linear algrebra course with applications to data science, based on the previous MAT227 but based in Python instead of Mathematica. This repository includes the old Mathematica notebooks for reference in the "Matrices and Geometry" folder, as well as the new Jupyter and Python resources in the "Python" folder.

## Using Python and Jupyter

Currently, we do not believe we will need to use any Python libraries except those which come standard in all Python installations (numpy, scipy, matplotlib, etc.). It would be ideal if the students and staff all used Python 3.7 for the sake of consistency, although most of the course will likely be backwards compatible with 2.7. If it would be helpful, I can include instructions for installing Python.

Using Jupyter is fairly straightforward. Assuming Jupyter is installed (and I believe that it also comes standard in most Python installations), you start it by navigating to the top level directory for your project in the command line (within Jupyter you can navigate down but not up), then run

    jupyter notebook

This starts a jupyter server and opens an editor in your browser. From the editor, you can open jupyter notebooks (file extension `.ipynb`), work on them, and save them. Then you can quit the session by clicking on logout in the corner.

## Using git and Github

Everyone who wants to contribute to this project should make an account on github and tell me their usernames so I can add them as contributors to the project. Once you accept the invitation, you can go to the project, and click on the green button "Clone or download." This should open a drop down menu which includes a link. Copy the link by clicking on the clipboard icon next to it. Then, in the command line, enter

    git clone url destination

where `url` is the url you just copied, and `destination` is the path to the folder you want to store this project in. So if you wanted this project to be in a folder off your home directory called `LinAlg`, you would use `~/LinAlg` as `destination`.

Now you have your own local copy of the repository, which can operate in parallel with the official version on github. To download changes someone else has made from github, use

    git pull

To check on the changes you have made in your local copy of the directory, use

    git status

To "stage" changed files for a commit (a commit is an official snapshot of the project, and is stored forever so you can go back to earlier versions if need be), use

   git add file

where `file` is the name of the file. To commit all your staged changes (which, again, you can check on with `git status`), use

   git commit -m "Title of commit"

It is generally good practice to make commit titles informative and to phrase them in the imperative, i.e. what will this commit do? It will "Fix formatting in README.md". And finally, once you've committed all your changes, you can push them to the Github repository with

    git push

The power of git and Github is partially in its ability to resolve differences between different peoples versions of the code, and there are more nuanced ways of handling things than just having everyone push their version of master each time they finish working (such as creating different brances, pull requests, etc.). However, I think that since we will likely not all be working on things at the same time, we won't have any issues as long as everybody pulls the latest version whenever they start working, and pushes their changes whenever they stop. 