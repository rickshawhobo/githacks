# Use git hacks

Alias to show a nice graph of git tree
```
    git log --oneline --graph --decorate --all --date=short --pretty=format:'%Cblue%cd %C(yellow)%h %C(cyan)[%an]%Creset -%C(auto)%d%Creset %s %Creset'
```

Alias to fetch the latest master and rebase your feature branch
```
    git fetch origin master:master && git rebase master
```

Alias to delete your stale local branches that have been rebase merged onto master
```
    git branch --merged master | grep -v 'master$' | xargs git branch -d
```

Git aware prompt tells you your current branch without constantly doing `git status`! Note this can be slow on VMs.

https://gist.github.com/eliotsykes/47516b877f5a4f7cd52f


Git autocomplete

https://github.com/bobthecow/git-flow-completion/wiki/Install-Bash-git-completion

