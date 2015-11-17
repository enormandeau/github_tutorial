# Git ![octocat](../images/git_logo.png)

## Overview of Git

Git is the revision control system behind GitHub. Git's role is to **make code
development more structured and to facilitate collaboration**.

## Graphical Interface vs Command Line

We will use the command line to understand the process. As there are many graphical
interfaces, this is a simple way to understand the necessary commands; later you
can use whichever graphical interface you choose.

## Using Linux from Terminal.com
**This section is optional**, if you have a computer with command line already prepared (Mac, Linux)
you may use Terminal or similar.

In order to try Git, we will be using virtual Linux machines available online.
To get started, head to
<a href="http://www.terminal.com" target="_blank">Terminal</a>
and create an account. From there, we will be using an already available
machine (or Snap). We will use
<a href="https://www.terminal.com/snapshot/987f8d702dc0a6e8158b48ccd3dec24f819a7ccb2756c396ef1fd7f5b34b7980" target="_blank">this snapshot</a>.
Leave the default settings as they are and press the `Start` button on the
bottom right.

Once the virtual machine is started, your screen will be divided in sections.
The only ones we want to use are `Terminal`, `Files`, and `Editor`, so you can
click on the other ones (`Browser` and `Chat`) to remove them. If you click on
the arrows after the name, the selected section will take the whole screen.

## Installing Git

Installing Git on the terminal snapshot is simple. Type the following code in
the terminal:

```
apt-get install git
```

If you are using your own Linux computer, you will need to add `sudo` in front
of the command:

```
sudo apt-get install git
```

To install Git on a Mac, Windows or non Debian based Linux distribution, follow
the instructions on the
[git installation page](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
However, if you are using Windows, the following parts of the tutorial may not
work for you. This is why we suggest that you use the Terminal.com option.

## Git setup

We now need to setup Git to integrate with GitHub. We follow the official
<a href="https://help.github.com/articles/set-up-git/"
target="_blank">GitHub setup help page</a>
for this.

We can also setup Git so it remembers our password for some time by following
<a href=""https://help.github.com/articles/caching-your-github-password-in-git/
target="_blank">these instructions</a>.

## Next section
In the next section, we will explore the standard Git workflow. We will be
using the `Planets` repository that you forked from here
<a href="http://github.com/enormandeau/planets"
target="_blank">here</a>.

### [04 - Basic Workflow](04_basic_workflow.md)

