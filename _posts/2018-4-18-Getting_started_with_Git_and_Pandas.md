---
layout: post
title: Git and Pandas, etc.
---
# A first blog post

Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.



## A quick guide to getting set up with Git, Pandas *Groupby*, and maybe Pycharm



### Git:

This tutorial should be useful to you if:

* you use a Mac
* you know some Command Line
* you have git installed and have started learning a little about git
* you have a Github account
* you'd like to get a first or second repo going and are looking for a robust workflow

I'm going to lay out a simple and robust workflow that's just right for getting started with Git. This assumes that you're fairly new to Git and aren't yet looking to collaborate or do any Git ninja moves. It's just to get something going.

The workflow of Git is something like this: you work on a `file`, presumably a piece of code, on your local machine, in some `folder/` directory,  `~/somepath/folder/` .  The basic workflow you'll learn about looks like this:

`local_file` - **push** -> `local_file` on Github



You'll want to start using Git because that's what grownup programmers do. There are two ways of using git here: 

1. Use git locally
2. Use git locally and "sync" your file to a repo in the cloud, say, on Github.

Option 1. is fine if all you cared about was version control: the ability to go back in time to a previous saved version should you get to a dead-end in your code that you'd like to back out of. Option 2. _additionally_ provides cloud-based backup of your code should your laptop get run over by a truck. So Option 2. is Option 1. and then some. Here we'll focus on Option 2:



Here are the steps:

* Go to github.com, sign in with your `username` if you're not signed in already, and click on **New repository** on the right-hand side of the page: 

  ![image-20180417081927246](/var/folders/f4/6zkljh491nq9hfnrnlplkryw0000gn/T/abnerworks.Typora/image-20180417081927246.png)

  You'll see a few options: 

  - Name your new repository. I'll just be referring to `repo` , but you could name it anything you want.
  - Choose Public if you don't mind people seeing the contents of `repo` and you want to keep this free of charge.
  - Go ahead and click "Initialize the repository with a README". It's good practice to have a README for yourself, your future self, and anyone else who might this. 

* In your new repository, `repo`, click on **Download or Clone**. A `link` to your new repo will pop up. Copy that `link`.

  ![image-20180417082044333](/var/folders/f4/6zkljh491nq9hfnrnlplkryw0000gn/T/abnerworks.Typora/image-20180417082044333.png)

  ​

* In your command line, go to the folder where you want to keep your local repository. If you don't yet have that folder, make one. I'll call it `local_repo_folder`:

  `cd ~/path_to_local_repo/local_repo_folder`

* Now, in the Command Line, type `git clone` and paste the `link` that you copied before: `git clone link`. A new folder named `repo` should appear *inside* `local_repo_folder`. This folder `repo` is your local clone! You can go ahead and do work in that folder, write 