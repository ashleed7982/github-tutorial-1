# GitHub Tutorial

_by Amanda Lum_

---
## Git vs. GitHub

### What is Git?

Git is a system which keeps track of changes to code as different versions, which becomes the history that you can go back to or view. It runs in the command line, and displays all of the directories (called folders) that hold your files.

### What is Github?

Github is a website that allows you to keep your code in the cloud. It lets people collaborate with each other, since you can publish your repositories (or make them private!) for others to work on and add to. You can see the changes you have made (insert image here)

### How are they different?
The difference between Git and Github is that Github needs to use Git, but Git can run on its own, offline. Github can track your changes more visually than Git does, and is more convenient to use to work with others.
---
## Initial Setup
### How to make a Github account:

This step is fairly intuitive: Go to [the website.](https://github.com/)

You will see a box where you can sign up (insert image here). Just put in your email, and choose a username and password that fit the character limits. You're done!

How to set up your IDE:
[Just check this website for assistance!](https://github.com/hstatsep/ide50)

By this point you have come in contact with the SSH key. But what is this? It is like a private key that, upon using, you can log in on a website. It is also used to identify different commits.
---
## Repository Setup
Once you have a directory, it's time to initialize it. When you initialize a directory (git init), it means you have chosen to do your project in this directory. You thus turn it into a repository. You must do this step first, otherwise you cannot use the other Git commands!

So, let's say that you make some changes to a file in your repository, and you want to save your hard work. You do (git add) in order to signify that you want to save these changes. This adds it to the stage, so it's ready for saving. You then do (git commit -m ""), which will save those changes. The -m is the precursor for the message you type in "", which is very important. Write a commit message; its kind of like a comment on your code so you can go back to the commits and see what changes you made in the past.
---
## Workflow & Commands
Git status is an essential command that you should be using often. Basically, use this command in between the process of adding, committing and pushing a file


---
## Rolling Back Changes
There are a few commands that can help you remove changes you have made to your code, just in case you make a mistake. These include git checkout --file, git reset HEAD file, git revert HEAD. 

Git checkout --file means that you are undoing any changes that were made in your working directory. If you were working with another person, and edited a file that you didn't mean to, you can avoid merge conflicts by using the command. There, everything is back to normal now!

Git reset HEAD file means that you are taking a file out of the stage. This can be used if you accidentally add all of the files, when you mean to add a specific one only. 

Git revert HEAD helps you go back to a prior commit. Use this command if you want to restart from a certain point.