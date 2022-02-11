
Download git for relevant OS from below url and install it.
[Download Git](https://git-scm.com/downloads)

Run below command in terminal/command prompt to check if git is installed or not :
```
$ git
```
After that command run you can see below output to terminal.
```
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]
```

Some basic linux commands :
```
$ ls => list all files/directory
$ ls -a => list all items with hidden files/folders 
$ mkdir directoryName => to make new directory
$ cd /path/to/any-folder => to change directory
$ touch fileName => to create new File
```

First initialize git using below command :
$ git init
Now you can see folder called .git and check it content using below command :
$ ls .git
Whatever changes now you make in current folder will be picked up git.

Now we will create new file README.md using below command :
$ touch README.md
Whatever changes made in folder will be check by below git command :
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	README.md - red color


Below command used to add files/folders which have not in history new file or changed/modified.
$ git add . 
$ git add README.md
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   README.md - green color

# image goes here for green status
Run below command to commit untracked or changed files/folders.
git commit -m " added README.md file "
Here -m means message for commit.
Now again run below command to check status.
git status