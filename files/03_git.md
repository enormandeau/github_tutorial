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
Leave the default settings as they are but click the two following boxes, found
near the bottom of the grey box on the right:

- Start as Temporary Terminal
- Auto-pause

This will ensure you will not have to pay for your machine during the tutorial.
It also means that after an hour, the virtual machine will destroy itself. This
is not a problem for our workshop since we can then simply start it again.

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
instances. Finally, even for more expansive instances, the pricing is very
competitive with other major cloud services available and you should at least
think of the potential use of Terminal in your research as a way of saving
research money on informatic equipment.

## Installing Git

Installing git on the Linux virtual machine is simple. Type the following code
in the terminal:

```
sudo apt-get install git
```

## Git setup

We now need to setup our Linux terminal to integrate well with GitHub. We
follow the official
<a href="https://help.github.com/articles/set-up-git/"
target="_blank">GitHub setup help page</a>
for this.

## Next section
In the next section, we will explore the standard Git workflow with some
exercices. We will create and modify a repository and learn the ropes of Git.

### [04 - Basic Workflow](04_basic_workflow.md)

