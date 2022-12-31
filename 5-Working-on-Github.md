## 4. Understanding GitHub :-

- We are going to do two thing.
  - Hosting our own project on GitHub to share.
  - Working on a remote repository by cloning.

- Go to GitHub and just create a repository.
- Copy the url to be attach for local project.

__To connect a new remote repository with your folder or local repository :__

```bash
git remote add origin _paste-url_
```

- Now this url is connected with folder.
- `remote` : means working with URLs.
- `add` : means adding new URL.
- `origin` : means what is the name of URL that you are going to add.
- By convention the urls of all repository are named as `origin`

__How to see all the urls that are attached to your folder :__

```cmd
git remote -v
```

__To push local changes to remote repository :__

- How to share the changes on URL's repository -

```bash
git push origin master
```

--------------->

## 4. Working on GitHub

**To check all remote links :**

```bash
git remote -v
```

**To add local repository to github :**

```bash
git remote add origin url
```

```bash
git -M master
```

**To push all content of local repository to github :**

```bash
git push -u origin branchName
```

- First our head should point on that branch

**To add collaborator to your existing repository :**

- If you want to multiple people work on a project
  - Make repo public then that person fork the project then they can make changes and push the files.
  - Another ways to work together is to add collaborator.
- Go `setting` -> `manage access` -> `add collaborator`
- Here collaborator can access your repository edit modify the changes.