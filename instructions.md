# Instructions

Open up `.bashrc` file and add the following

```
#aliases
if [ -f ~/.bash_aliases ]; then
  . ~/.bash_aliases
fi
```

If you have setup an **ssh key** for GitHub, also add this to the `.bashrc` file.

```
# loading ssh github ssh key
eval `ssh-agent -s`
ssh-add ~/.ssh/github
```

If you have installed **tmux** add this line to the `.bashrc` too.

```
tmux
clear
```

## Git Aliases

```
git config --global alias.co checkout
git config --global alias.cm "commit -m"
git config --global alias.s status
git config --global alias.p pull
git config --global alias.cob "checkout -b"
git config --global alias.f "fetch --all --prune --tags"
git config --global alias.l "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"
git config --global alias.db "branch -d"
git config --global alias.fdb "branch -D"
git config --global alias.dbr "push -d origin"
```
