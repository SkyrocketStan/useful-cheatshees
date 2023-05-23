
## Git aliases

To see all your aliases, list your configuration with git config:

```
$ git config --global -l

alias.co=checkout
alias.br=branch
alias.ci=commit
alias.st=status
alias.unstage=reset HEAD --
alias.last=log -1 HEAD
alias.hist=log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short
alias.cm=commit -m

```
1. git push (git p)
    > $ git config --global alias.p 'push'

2. git status (git st)
    > $ git config --global alias.st 'status'

3. git commit (git cm "A nice commit message")
    > $ git config --global alias.cm 'commit -m'

4. git config list (git gl)
    > $ git config --global alias.gl 'config --global -l'



## Global .gitignore
    > git config --global core.excludesfile ~/.globalignore


## Remove from git

#### Remove directory from Git but NOT local
```
git rm -r --cached <folder_name>
```

#### Remove directory from Git and local
```
git rm -r one-of-the-directories // This deletes from filesystem
```
