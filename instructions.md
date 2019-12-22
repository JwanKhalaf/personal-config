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
