# _Benjamin Novik's Github Tutorial Project_
---
Hello! This file is meant for people who are new or trying to review Git and Github. I have been using Github since September 2019 for a couple months. I believe that I have a great enough understanding to try and teach others. If you used Git and Github before you might just learn a new trick or two.  

### Git VS Github
___
Git and Github are two seperate things but you need Github to use Git. You do not need Git to use Github.  

_What is Github?_ Github is a cloudbased tool or service used to help creators share, store and collaborate with each other. It is popular for its ability to track changes made to a file. The 'creators' or the user is able to upload their project(s) to be saved onto the Github server. If you are doing a group project with other people, Github will allow you to share it so that other people can edit and make changes to the file.  

_What is Git_? Git is designed to work hand and hand with Github. It is installed into your local or your computer system. Your local is like your hard drive. Its where all of your files, directories, downloads, images etc are located. You would use the command line to navigate through your files and projects efficiently. When Git is activated within your directories they become repositories. You can then begin to use Git to track your changes to then upload them to Github for a safe place to save your files and projects.

### Initial Setup
___

Git and Github must sound super useful and awesome but you probably do not know how to set it up so I am going to try and explain that to you.  

First off you are going to have to make a Github account on [Github](github.com/). This is pretty straight forward. Your going to need an email, a unique username and password that is strong (recommended). Once you have created your own Github account you can follow the directions [here](https://github.com/hstatsep/ide50) to set up your IDE. Follow all of the steps in their correct orders and make sure to read it all carefully.  

It is important to set up the SSH key because thats how your going to link your projects between your IDE and Github. Your SSH Key is your own very unique key that will allow you to create repositories, clone, and fork from Github to your IDE.

### Setting up your First Repository
___

You have finally set up Git in your IDE and now you have your Git and Github linked. Whats next? Making your first repository is what's next! By creating a repository you are allowing for Github to track the chanegs made to your specific files and projects, which was the point from the very beginning.  

To start off, you are going to want to make a new directory in your IDE. Lets name it 1st-repository. Then you are going to `cd` or _change directories_ (Your going to `cd` into your first repo).  

You are then going to initialize the direcrtory to create it into a repository by simply typing the command : `git init`. If you ever git init in the wrong directory(s) you can simply uninitialize with the command `rm -rf .git`. Then you are going to make a file in your new repository with the command `touch` (filename). Then you will add something to the file, could be text an image etc. You are going to then add the file to the staging branch to get it ready to be commited. You will do this by typing the commands `git add (name of the file you want to add)`, then `git commit -m "message"`. The message will be a short summary of the changes you have made to the specific file (3-8 words is great).  

Now that you have commited your file it is time to make a repsoitory on Github to then link your local to the cloud. Goto [Github](github.com/) and goto your home screen. In the top right corner you will see a "+" symbol. Click it and a drop menu should appear. You will then see new repository. Click that too. You are then going to name that repository with the exact same name form your IDE. In this case it would be 1st-repository.  

A panel should show up with a bunch of giberish. At the top make sure that the SSH Key option is selected. You are then going to type the following commands into your IDE. `git remote add origin git@github.com:(YOUR username)/(YOUR repository name : 1st-repository)` then you will type `git push -u origin master`. Now you are finished, you have just created your first repository. Now whenever you want to push your local changes to the cloud (for this repository) you just type `git push`. (After commiting a change of course)

### Ongoing and Workflow Commands
___

Some simple must know commands when using git in your local!

* `git status` Will tell you the status of a current repository letting you know what files you have ready to commit. The file will be in red if it is not being commited and green if it is being commited. This command is heavily recommended to avoid mistakes before you commit.  

* `git add (file name)` Adds a file (of your choice) to the "stage" to be ready to be commited.

* `git reset (file name)` Removes a file (that has already been added) from the stage if you have mad a mistake or just changed your mind about commiting that file.

* `git commit -m "(commit message)"` Commits a file to be saved as a change. Once this command is typed, all the changes done to it will be tracked to a commit message of your choice. Try and make a short and simple commit message to give your future self a better idea on what you changed in that file.

* `git push` Pushes your repository to github or to the cloud. This could be seen as a sort of save tactic since your files are stored in your local, which is one place. Pushing moves it to the cloud or the github servers keeping it secure just in case your local gets damaged or inaccessible.  

### Rolling Back Changes
___

Now that you are familiar with Git and Github, you are going to probably make some mistakes. Like commit the wrong thing, add the wrong thing etc. You need to know how to undo or rollback changes. If you ever want to uncommit something its simple. Your going to type the command `git reset HEAD~`. This will rest your most recent commit and unstage your files. If you want to keep your files staged then use the command `git reset --soft HEAD~`. If you have already pushed your commit to github and you want to take it back you can, with the command `git push origin master --force`. This command will undo the push and the commit but you must have revision permissions on the file in order to use it. You can not just mess with other people's files and projects.
