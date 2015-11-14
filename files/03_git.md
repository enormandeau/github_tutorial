# Git ![octocat](../images/git_logo.png)

## Overview of Git

Git is the revision control system behind GitHub. Git's role is to **make code
development more structured and to facilitate collaboration**.

## Graphical Interface vs Command Line

- We will use the command line to understand the process
- This will help you understand the processes better
- It is easier since there are multiple Graphical Interfaces available
- You can use a Graphical Interface in the future

## Using Linux from Terminal

In order to try git, we will be using virtual Linux machines available online.
To get started, head to
<a href="http://www.terminal.com" target="_blank">Terminal</a>
and create an account.  From there, we will be using an already available
machine (or Snap). We will use
<a href="https://www.terminal.com/snapshot/987f8d702dc0a6e8158b48ccd3dec24f819a7ccb2756c396ef1fd7f5b34b7980" target="_blank">this snapshot</a>.
Leave the default settings as they are and press the `Start` button on the
bottom right.

Once the virtual machine is started, your screen will be divided in sections.
The only ones we want to use are `Terminal`, `Files`, and `Editor`, so you can
click on the other ones (`Browser` and `Chat`) to remove them. If you click on
the arrows after the name, the selected section will take the whole screen.

**Note:** Terminal gives you 1 cent of credit when you create an account. As
long as your balance remains positive, you can use the services. Since micro
instances cost 0.6 cents per hour and the billing is done on an hourly basis,
this means you get two free hours at the start, which should be enough to go
through the tutorial. However, the micro instances are really cheap and adding
one dollar to your balance will give you more than a hundred hours to use micro
instances. Finally, even for more expensive instances, the pricing is very
competitive with other major cloud services available and you should at least
think of the potential use of Terminal in your research as a way of saving
research money on informatic equipment.

## Installing Git

Installing git on the Linux virtual machine is simple. Type the following code
in the terminal:

```
apt-get install git
```

If you are using your own computer, you will need to add `sudo` in front of the
command:

```
sudo apt-get install git
```

## Git setup

We now need to setup git to integrate with GitHub. We follow the official
<a href="https://help.github.com/articles/set-up-git/"
target="_blank">GitHub setup help page</a>
for this.

We can also setup git so it remembers our password for some time by following
<a href=""https://help.github.com/articles/caching-your-github-password-in-git/
target="_blank">these instructions</a>.

## Next section
In the next section, we will explore the standard Git workflow with some
exercices. We will create and modify a repository and learn the ropes of Git.

### [04 - Basic Workflow](04_basic_workflow.md)

