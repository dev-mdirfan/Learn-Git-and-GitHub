# Use Cases :
* You want to collaborate with other people.
* Want to add more feature on your projects.
* Want to go previous versions of your projects (basically saving the history of your projects).
* You want to contribute in open source or in a project.

# What is Git :
* Git & GitHub allows us to maintain the History of projects.
* At what particular of time which person made which change where in the project.

# GitHub :
* It is a platform or an online website that allows us to host our repositories.

## What is Repository :
* It is just a folder where all changes are saved.

## Terminal ?
* Terminal allows us to manipulate the file structure using command.

## .git file :
* Entire history of your working on a folder stored in .git file.

#### Note :
To paste in git command line press : shift + Insert Delete

# Using Command Line :
### How to make a folder? : (make directory)
    mkdir project
### How to go inside a folder? : (change directory)
    cd project

### How to see all content of a folder? : (list)
    ls

### How to initialize a folder as .git? :
    git init

### How to see all hidden files like(.git)? :
    ls -a

### How to see what content inside hidden file .git? :
    ls .git

### How to create a new file? :
    touch name.txt

### How to remove/delete a particular file? :
    rm -rf name.extension

### How to check whats going in present working directory or show the all changes in present? :
    git status

### How to put all new files which is untracked into .git for tracking? :
    git add .
### OR To add individually file by name into staging area? :
    git add file.name

### How to capture a snapshot of your work or to save your work? :
    git commit -m "your message"

### How to open any file and write? :  (vim)
    vi file.name

### How to display content of a file? :
    cat file.name

### How to get back unstage from staged without having commit? :
    git restore --staged name.txt

### where you can see all commit that made in history? :
    git log

### How to remove a commit from the history copy the hashID from (git log) :
    git reset paste_hashID

#### Note :
* You can't remove a commit from middle.
* All above commit will remove where you reset.

### How to go in previous commit ou changes without commit and also don't want to loose present change : (Back in the project)
    git stash

### How to come back that changes (i.e. backstage) : popping stash
    git stash pop

### How to clear stash which is commit : clearing stash
    git stash clear

### How to connect a new remote repository with your folder (local repository) :
    git remote add origin https://url

### How to check all url attached to your folder :
    git remote -v

### How to push local changes to remote repository :
    git push origin master

# What is branch? :
* Branch
![Learning branch](Learn-Branch.png)
### How to create a new branch :
    git brach name

### How switch to another brach : (now your head is pointing to other branch)
    git checkout name


#### Note :
* Whenever you working on some other feature or resolving a bug always create a separate branch.