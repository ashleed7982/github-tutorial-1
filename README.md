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

<<<<<<< HEAD
<<<<<<< HEAD
You will see [a box.](https://raw.githubusercontent.com/Amandal4012/github-tutorial/master/Screen%20Shot%202019-11-27%20at%209.26.18%20AM.png) Just put in your email, and choose a username and password that fit the character limits. You're done!
=======
You will see [a box.](http://www.cs.williams.edu/~dbarowy/cs334s18/assets/tutorials/github/github-login.png) Just put in your email, and choose a username and password that fit the character limits. You're done!
>>>>>>> 8ddb995... Swap content of Repo setup with Workflow & Commands + add to both
=======
You will see [a box.](http://www.cs.williams.edu/~dbarowy/cs334s18/assets/tutorials/github/github-login.png) Just put in your email, and choose a username and password that fit the character limits. You're done!
>>>>>>> 8ddb995... Swap content of Repo setup with Workflow & Commands + add to both

How to set up your IDE:
[Just check this website for assistance!](https://github.com/hstatsep/ide50)

By this point you have come in contact with the SSH key. But what is this? It is like a private key that, upon using, you can log in on a website. It is also used to identify different commits.
---
## Repository Setup
Once you have a directory, it's time to initialize it. When you initialize a directory (git init), it means you have chosen to do your project in this directory. You thus turn it into a repository. You must do this step first, otherwise you cannot use the other Git commands! Do git add . and git commit -m "[message]". Put a message so you can look at it and understand the changes you made to your file! Create a new repository on Github (insert image here) and use the same name from your repository in your cs50 ide to this one. Then, you need to make this new repository your remote, essentially linking the two so changes in your cs50 ide can be moved onto the remote. You can do this by using git remote add origin [url], which creates the link. After that, once you make any changes do git push -u origin master. This pushes the changes to the remote now. From now on, you can do git push, which will do the same and will be easier to type!
---
## Workflow & Commands
Git status is an essential command that you should be using often. Basically, use this command in between the process of adding, committing and pushing a file, and it will tell you if your files are to be added, committed, and if they are already pushed, and no changes have been made since your last push.

You do (git add) in order to signify that you want to save these changes. This adds it to the stage, so it's ready for saving. You then do (git commit -m ""), which will save those changes. The -m is the precursor for the message you type in "", which is very important. Write a commit message; its kind of like a comment on your code so you can go back to the commits and see what changes you made in the past. Git push means that you are officially publishing those changes to your Github remote. Your local changes are transferred to the remote, where others can easily interact with them.

---
## Rolling Back Changes
There are a few commands that can help you remove changes you have made to your code, just in case you make a mistake. These include git checkout --file, git reset HEAD file, git revert HEAD. 

Git checkout --file means that you are undoing any changes that were made in your working directory. If you were working with another person, and edited a file that you didn't mean to, you can avoid merge conflicts by using the command. There, everything is back to normal now!

Git reset HEAD file means that you are taking a file out of the stage. This can be used if you accidentally add all of the files, when you mean to add a specific one only. 

Git revert HEAD helps you go back to a prior commit. Use this command if you want to restart from a certain point.