## 3. Git Commands :-

### Make project

- Now you can make any project which you want to code in python, java, c, c++, web-d.

__Check status: which files have been changed :__ modified, added or deleted

```bash
git status
```
  - It show status of all changes that you have made in present of working directory.

__Initialize a folder as git repository :__ It creates .git

```bash
git init
```

### 1. What is .git file ?

- Where is the entire history is being stored ?
- Entire history of your working on a folder are stored in another folder named as `.git` file that git provides us.
- dot files are hidden.

### 2. Understanding Staging Area and Commit :-

- Imaging you are in wedding photographer want to take picture of the people.
  1. First step is the guest go on the stage whose photo has not been taken.
  2. The photographer will take picture.
  3. Then they will exit the stage.
  4. Now, Their picture will be permanently saved in the history of photo album.
- Git relates as, the guest whose photo has not been taken yet, they are known as __Untracked Files.__
- Next step is to take photo of that files so that it can saved in photo album by -


![Concept of staging Area](/images/Staging-Area.jpg)

- Staging Area : where you hold the changes before you make commit.

__Add all file in staging area :__ It hold the changes before you commit.

```bash
git add .

# Add by individual names
git add file.name
```
  - It put all new files which is untracked into `.git` for tracking.
  - It adds only one file into staging area.

__Commit after staging area :__ Provide message to that save the changes as commit.

```bash
git commit -m "your message"
```
  - This message should be meaningful.
  - This is capturing a snapshot of your work or to save your work by telling the message.

__Open any file and write in the command line :__ vim
```bash
vi file.name
```
  - Make Your Change
  - To exit from editor in git bash:- `Esc` + `:` + `wq`

__Unstage from staged without making commit :__

```bash
git restore --staged name.txt
```
  - If you have add to staging area you can unstage by `git restore --staged FileName`

__See all commit of history :__

```bash
git log
```
  - Every commit generated HashID.
  - To clear the terminal : `Ctrl` + `l`

__To go on particular commit :__

```bash
# switch to comment
git checkout paste_commit_hashID

# switch to branch
git checkout master
```
  - Here, with HashID created different branch.
  - checkout command used to switch the branches and commits.

__Want to remove present commit that you made :__

- How to remove a commit from the history, copy the hashID from (git log) ?
- Copy the below commit Hash ID

```bash
git reset paste_commit_hashID
```

- You can not remove a particular from middle, because each commit has HashID and each commit build on top of other commit. But you can unstage all above commits of that commit where you want to reach.

#### Note -

- You can't remove a commit from middle.
- All above commit will remove where you reset.

### 3. Stash

__How to go in previous commit you changes without commit and also don't want to loose present change (Back in the project) :__

- if you made changes and added to staging area and not commit yet, then want to work as a clean working space without losing that adding in stage area -

```bash
git stash
```

__How to come back that changes (i.e. backstage) popping stash :__

```bash
git stash pop
```

__How to clear stash which is commit (clearing stash) :__

- When you have stash the changes and want to clear that stash -

```bash
git stash clear
```
