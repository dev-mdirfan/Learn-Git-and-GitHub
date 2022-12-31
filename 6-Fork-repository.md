## 6. Fork repository :-

- Fork a existing repository, it makes copy of that repository in your account.

**To go on previous directory :**

```bash
cd ..
```

- Clone that repository on local.

**To clone the remote repository :**

```bash
git clone <repo url>
```

- Make changes on them.

```bash
# To edit the file in vim editor
vim <file name>
```

- to write/edit press "i"

```bash
# To see the content fof file
cat <file name>
```

### Pull Request :-

- When other user push the files to your repository then pull request is generated, you have to merge with your verification.
- confirm the `merge`.

**Then all you have to repeat and again repeat :**

- Repeat.

----------------->


## 6. Forking : Working with existing project on GitHub

- what is way to contribute to an organization on a repository.
- By Forking (copy) you take project on your own account by clinking on `Fork` section in GitHub.
- This is not reflect in the main project until and unless the people who have approval for this project can merge your changes via pull request.

__How to clone a repository (the forked project to local) :__

```bash
git clone https://url
```

__Note :__

- If your repository of your account name of that is going to be origin.

### What is Upstream URL :-

- From where you have fork the project that is known as Upstream URL.

__How to add Upstream URL :__

```bash
git remote add upstream https://upstream_url

# check remotes
git remote -v
```

- You are ready to pull request.

### Pull Request

- How to push code of a branch of your account to upstream repository i.e. Pull request.
- When you create a copy (fork) and make any change how do you make sure that this change is visible in the main project, you have to request via a pull request then people will review your code, suggest some changes you will make those changes and when this is merged your sample changes that you made in your own account fork in any branch that will visible in main project in the main branch.

#### Note :-

- You can not push your code  directly on upstream url, it will give an error like (git push upstream branchName), you don't have access but you have access to origin url -

```bash
# Gives Error in adding to upstream
git push upstream branchName

# add to your own forked repo
git push origin branchName
```

- Then you need to pull request from `pull request` section in GitHub.
- When you have pushed again your changes to origin that you have created already pull request it will generate 2nd commit on that pull request.
- This is reason why you should never commit on main branch. Imagine you working on 10 feature and for every feature you create just one request how difficult it would be to review your code to have your discussion all 10 different features are just in one pull request hta is why for every new feature, every new bug create a new pull request or different branch.
- In simple language one branch can open one pull request at a time.
- If you want to open different pull request for that you will need to create new branches.
- If many people working and created many pull request that means everyone working on own pull requests.

__Removing a commit from the pull request by force pushing to it :__

```bash
# copy hashID the below commit from git log
git reset hashID

# Or this can be done with hard
git reset --hard hashID

git add .

git stash

# You have to force push because you have different commit in remote repo
git push origin branchNme -f
```

__When online repository contain a commit that local does not contain that commit then you have to force push :__

```bash
git push origin branchName -f
```

- Finally owner of upstream url can merge the that pull request.

### Fetch Upstream

- Now your forked repo not updated because you have pull request and that merged in upstream repo, this is one ahead step to your forked repo. then you have to fetch the upstream repo.
- How do you make sure main branch of the Upstream and your own forked main branch always maintain for that : (Fetch Upstream)
- You can use one click in github in top. You can use `Fetch upstream` from GitHub.

#### Second way to do that -

```bash
# you have to head on main branch
git fetch --all --prune

# reset the main branch of origin to the main branch upstream
git reset --hard upstream/main

git log

git push origin main
```

#### OR another way (3rd) :-

```bash
# Fetching using pull
git pull upstream main

git log

git push origin main
```

#### Note

- When ever you create a new branch, it will created from `head` make sure you __main__ or __master__ is  up to date before creating a new branch.