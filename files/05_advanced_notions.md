# Advanced notions

This section contains notions and examples that are more advanced. The goal is
not to be exhaustive about it but just to make you aware that these subjects
exist so that you know about them when you may need them in the future.

**NOTE:** This section is still a work in progress.

## Creating aliases

After a while, typing the git command may feel tedious. Creating a few short
aliases can make your life easier. Here are a few examples you could include
in your `.bashrc` file:

```
# Git
alias gs='git status'
alias ga='git add'
alias gb='git branch'
alias gi='git commit'
alias gii='git commit -m'
alias gd='git diff'
alias gdd='git diff --color-words'
alias gc='git checkout'
alias gp='git push'
alias gg='echo ">>> Branches"; \
    git branch; \
    echo; \
    echo ">>> Graph"; \
    git log --oneline --color --graph --all --decorate'
```

## Forking and pull requests

## Working with branches

## Reseting

## Creating and pushing tags

## Cherry picking

## Creating aliases for common Git commands

## Next section
In the next section...

### [06 - Conclusion](06_conclusion.md)

