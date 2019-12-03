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

First of all you are going to have to make a Github account on [Github](github.com/). This is pretty straight forward. Your going to need an email, a unique username and password that is strong (recommended). Once you have created your own Github account you can follow the directions [here](https://github.com/hstatsep/ide50) to set up your IDE. Follow all of the steps in their correct orders and make sure to read it all carefully.  

It is important to set up the SSH key because thats how your going to link your projects between your IDE and Github. Your SSH Key is your own very unique key that will allow you to create repositories, clone, and fork from Github to your IDE.

### Setting up your First Repository
___

You have finally set up Git in your IDE and now you have your Git and Github linked. Whats next? Making your first repository is what's next! By creating a repository you are allowing for Github to track the chanegs made to your specific files and projects, which was the point from the very beginning.  

To start off, you are going to want to make a new directory in your IDE. Lets name it 1st-repository. Then you are going to `cd` or _change directories_ (Your going to `cd` into your first repo).  

You are then going to initialize the direcrtory to create it into a repository by simply typing the command : `git init`. Then you are going to make a file in your new repository with the command `touch` (filename). Then you will add something to the file, could be text an image etc. You are going to then add the file to the staging branch to get it ready to be commited. You will do this by typing the commands `git add (name of the file you want to add)`, then `git commit -m "message"`. The message will be a short summary of the changes you have made to the specific file (3-8 words is great).  

Now that you have commited your file it is time to make a repsoitory on Github to then link your local to the cloud. Goto [Github](github.com/) and goto your home screen. In the top right corner you will see a "+" symbol. Click it and a drop menu should appear. You will then see new repository. Click that too. You are then going to name that repository with the exact same name form your IDE. In this case it would be 1st-repository.  

A panel should show up with a bunch of giberish. At the top make sure that the SSH Key option is selected. You are then going to type the following commands into your IDE. `git remote add origin git@github.com:(YOUR username)/(YOUR repository name : 1st-repository)` then you will type `git push -u origin master`. Now you are finished, you have just created your first repository. Now whenever you want to push your local changes to the cloud (for this repository) you just type `git push`. (After commiting a change of course)