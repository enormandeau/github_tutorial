# Git ![octocat](../images/git_logo.png)

## Overview of Git

Git is the revision control system behind GitHub. Git's role is to **make code
development more structured and to facilitate collaboration**. Git was written
by Linus Torvald, who is know for having written the Linux kernel.  The Linux
kernel developers were using a revision control system but Linus felt a new
tool was needed. Between two kernel versions, he thus wrote Git to replace the
revision control tool they were using.

## Graphical Interface vs Command Line

In this tutorial, we will use the command line to understand the process of
using Git. The terminal brings us closer to the core Git commands and so leads
to a better understanding. As there are many graphical interfaces and since
they vary from OS to OS, using the terminal is also simpler for teaching;
Everybody is using the same interface. Later you can use whichever graphical
interface you choose.

## Installing Git

Installing Git on Debian-based Linux distribution (eg: Ubuntu, Mint) is simple.
Type the following code in the terminal:

```bash
apt-get install git
```

If you are using your own Linux computer, you will need to add `sudo` in front
of the command:

```bash
sudo apt-get install git
```

To install Git on a Mac, Windows or non Debian based Linux distribution, follow
the instructions on the

<a href="https://git-scm.com/book/en/v2/Getting-Started-Installing-Git" target="_blank">git installation page</a>
However, if you are using Windows, the following parts of the tutorial may not
work for you.

## Setting up Git

We now need to setup Git to integrate with GitHub. We follow the official
<a href="https://help.github.com/articles/set-up-git/"
target="_blank">GitHub setup help page</a>
for this.

We can also setup Git so it remembers our password for some time by following
<a href=""https://help.github.com/articles/caching-your-github-password-in-git/
target="_blank">these instructions</a>.

## Next section
In the next section, we will explore the standard Git workflow. We will be
using the `Planets` repository that you forked from
<a href="http://github.com/enormandeau/planets"
target="_blank">here</a>.

### [04 - Basic Workflow](04_basic_workflow.md)

