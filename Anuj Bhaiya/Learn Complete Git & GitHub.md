### To initialize a folder as git repository :
    git init

### To check hidden content of a folder :
    ls -a

### To check the status like what changes are made or modification are done :
    git status

### To go in Staging Area : 
* It basically hold the changes before you commit.

        git add file.name

![Concept of staging Area](Staging-Area.jpg)

### To commit from staging area :
    git commit -m "your message"

### To check how many have commit are :
    git log

### To clear the terminal :
* `Ctrl` + `l`

### To go on particular commit :
    git checkout HashID
* Here, with HashID created different branch

### To back on present from that particular commit :
    git checkout master

### To check how many branch :
    git branch

### To create new branch :
    git branch branchName

### To create new branch and point hea to that branch :
    git checkout -b branchName

* **Example- branchName** anuj/multiply

### To merge a branch to other branch :
    git merge anuj/multiply
#### Note : 
* Your head must point to another branch in which you want to merge.

### To ignore the files in git/github :
    touch .gitignore
* put the files name inside the `.gitignore` for ignore that file.

### To add local repository to github :
    git remote add origin url

### To push all content of local repository to github :
    git push -u origin branchName

### To push other branch :
* First our hea should point on that branch

        git push -u origin branchName

### To add collaborator to your existing repository :
* Go `setting` -> `manage access` -> `add collaborator`
* Here collaborator can access your repository edit modify the changes.

### To fork a repository :
* Fork a existing repository.
* Clone that repository on local.
* Make changes on them.
* Pull Request.
* Repeat.