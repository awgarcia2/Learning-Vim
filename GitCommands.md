# Git Commands
## Setup
First make sure that you have git installed. If you need to install it you can use command:

```sudo apt-get install git```

Once git is installed you might want to perform some additional setup steps such as `git config` and a ssh-key. See [GitSetup](https://github.com/albertgarcia7149/Learning-Vim).

## First Repo
You can create a local repository by using the command:

```git init```

This will put all the necessary files in the directory so you can push to github later.

Now you can create some files to be in your repository.

Once you have some files you need to move them to the staging area. The staging area is where you place all of the files that are ready to be committed. 

You can add a file to the staging area with command:

```git add <file>```

or add all files in the directory with:

```git add .```

Once you have the files in the staging area you can make a commit with command:

```git commit -m "<changes>"```

You can ommit the `-m "<changes>"` but it is good practice to make notes on the changes.

Once you have made a commit you can push your changes to github with command:

```git push```

Another useful command is:

```git status```


which displays the state of the working directory abd the staging area.


Now you have a basic handle on Git.

## Branching
