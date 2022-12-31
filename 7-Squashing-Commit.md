# 7. Squashing Commits :-

- If you have lots of commit and you want to merge into one commit.
- One way to do that is -> `reset commitHashID` -> commit again.

__How to merge all of commit into one commit :__

- Using rebase :
  - Copy Last Commit Hash ID

```bash
# -i means the interactive environment
git rebase -i paste_HashID
```

- All the above commits above it, you can either __squash__ or __pick__.
- All squash commit are added into above pick commit.
- So which you want to merge write :- __s__ (It will add into above commit which have pick)
- Or you want to leave that commit as it is :- pick
- To add the new commit message : `Esc` + `:` + `x`
- Write "Your message"
- exit the editor : `Esc` + `:` + `x`