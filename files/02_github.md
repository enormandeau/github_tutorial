# GitHub ![octocat](../images/Octocat_small.png)

## A graphical overview of GitHub

In this section, we look at the different parts of GitHub and at a user
account.

### Main Page

When you do not have an account the GitHub, the main page offers you to search
among the existing projects or to create an account.
<a href="http://github.com/" target="_blank">Main page</a>
Otherwise, it displays the activity of accounts and projects you are following.

### User Page

The user pages show an avatar of the users and list their projects. Only the
most popular projects are listed but by clicking on the `repository` tab, you
can access all of a user's projects.
<a href="http://github.com/enormandeau" target="_blank">User page</a>

### Projects (or repositories)

In Git parlance, projects are called repositories. Repositories contain folders
and files, as well as all the history information about the project, like the
changes that were applied, when, by whom, and all the versions all the files
that have existed throughout the project's existence.
<a href="http://github.com/enormandeau?tab=repositories"
target="_blank">Projects repositories</a>

### Example Project

Let's look at an example project:
<a href="http://github.com/enormandeau/meditation-timer"
target="_blank">Example project</a>

This project contains a `data` folder with a text file, a main script
(`planets.sh`), and a `README.md` file. The `README.md` file is very important.
It is used by GitHub to create the page that describes the project. It is very
useful to have such a `README.md` file and to use it to describe the project,
how to install or use the scripts, and display the license information.

## Creating an account

If you do not already have a GitHub account, we will now create one so that you
can follow the tutorial. Please fill the following sections:

- Login name
- Email address
- Password

Then choose the `Free` plan and click on `Finish sign up`.

Congratulations! You now have a GitHub account. You will need to verify your
email account before you can use it, so please do so now.

## Creating a test project

Once you have validated your account, creating a new project is easy: 

- Click on the `+` sign in the upper right and select `New repository`
- Name your repository `test`
- Add a short description if desired
- Click on `Initialize this repository with a README`
- Click on the green `Create repository` button

Your empty directory has been created. You can now modify it, either directly
from GitHub in your browser or on your computer.

## Editing the README file from GitHub

To modify the `README.md` file directly from GitHub:

- Click on the `README.md` link
- Click on the pen in the upper right portion of the file
- Copy the following text to the `README.md` file:

```
## This is a level 2 title

- This
- is
- a
- list

### This is a level 3 title

Here is a command: `echo "Hello!"`
```

  - Click on the `Commit changes` button on the bottom
  - Your changes are now effective and visible!

## Forking a project

During this Git and GitHub tutorial, we will use a training project about the
plantes of the solar system. We will use a simple bash script and small text
files. You do not need to know how to program in bash to follow this example.
We will introduce the changes to the code and the data files together. To get
the repository:

- Go to
<a href="http://github.com/enormandeau/planets"
target="_blank">this repository on GitHub</a>
- Click on the `Fork` button near the upper right of the screen

This will create a copy of the `Planets` repository for you. You own this copy
and will be able to modify it during the tutorial.

## Next section

In the next section, we will set up a Terminal.com account from which we will
install Git and set it to work with your GitHub account.

### [03 - Git](03_git.md)

