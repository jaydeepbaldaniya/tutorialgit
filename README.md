
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
$ cat fileName => Concatenate open file, read it and close it
```

First initialize git using below command :
```
$ git init
```
Now you can see folder called .git and check it content using below command :
```
$ ls .git
```
Whatever changes now you make in current folder will be picked up git.

Now we will create new file README.md using below command :
```
$ touch README.md
```
Whatever changes made in folder will be check by below git command :
```
=> $ git status
On branch master
No commits yet
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	README.md - red color
```

Below command used to add files/folders which have not in history new file or changed/modified.
```
=> $ git add . 
=> $ git add README.md
On branch master
No commits yet
Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   README.md - green color
```

Run below command to commit untracked or changed files/folders.
```
=> $ git commit -m " added README.md file "
[master (root-commit) 82f1dcd]  added readme file
 1 file changed, 62 insertions(+)
 create mode 100644 README.md
```
Here -m means message for commit.
Now again run below command to check status.
```
=> $ git status
On branch master
nothing to commit, working tree clean
```

Now again change readme and add it.
```
=> $ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md
no changes added to commit (use "git add" and/or "git commit -a")
=> $ git add .
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   README.md
=> $ git commit -m " changes in readme file "
[master 31606da]  changes in readme file
 1 file changed, 13 insertions(+)
```

