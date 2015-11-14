# Advanced notions

This section contains notions and examples that are more advanced. The goal is
not to be exhaustive about it but just to make you aware that these subjects
exist so that you know about them when you may need them in the future.

## Ignoring certain files

Git uses `.gitignore` files to know which files should be tracked and which
should be ignored. Git is very good at tracking small text files. It is very
bad for tracking large binary files, like PDFs, compressed files or images. If
you expect your project folder to contain such files during your normal use but
do not want to track them, you should use the `.gitignore` file to exclude
them.

Here is the content of a fictive `.gitignore` file that ignores temporary
files, PDFs and images:

```
*.PDF
*.gif
*.jpeg
*.jpg
*.pdf
*.png
*.swp
*.tiff
*~
```

## Getting remote changes

If you work on a project from two computers, for example one at work and one at
home, you will need to synchronize the changes made to your project before you
can continue working. Let's say you have the same project on two computers, A
and B, and you work on computer A. Tomorrow, when you are on computer B, the
project folder is not up to date. To bring it up to date, you need to use the
following command:

```
git pull
```

If you work on one computer at a time and push your changes to GitHub, this
approach will work very well as long as you `git pull` before each session. On
the other hand, if you work on the project in computer A for some time and,
during the same period, you also work on the project on computer B, it is
possible that the changes will be impossible to merge automatically. In these
more complicated cases, you will need to do a manual merge. This is outside the
scope of this tutorial but see the Ressources in the Conclusion section.

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

When you fork a project on GitHub, you can then clone it using `git clone
<URL>`. If you make changes and push them back, you can then go to your forked
repository and click the `Pull request` on the right side of the screen to
initiate a pull request. This means that the original author of the repository
will receive a request to include your changes into his code. This is one of
the primary ways to collaborate at developing code with GitHub.

## Next section

In the next section, we conclude this brief tutorial.

### [06 - Conclusion](06_conclusion.md)

