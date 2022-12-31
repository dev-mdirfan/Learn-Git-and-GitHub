# 2. Set Configuration

- If you install first time then you have to set config name and email so that, anywhere you made change anyone can know who is the author.

__Set your configuration of your account :__

```s
git config --global user.name "Your Name"
git config --global user.email "yourmail@gmail.com"
```

__See Account information :__

```bash
git config --global user.name
git config --global user.email
```

__Change your information :__

- It opens vim editor to edit the information.

```bash
git config --global --edit
```

__Exit the VIM Editor :__

- To exit editor : `Esc` + `:` + `wq`
