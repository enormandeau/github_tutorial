# Basic Workflow

## Working on a project

Now that you have an active project, `Planets`, to work with, we will need to
download it on your Terminal.com terminal to work on it.

## Downloading a repository from GitHub

To get a local copy of your project, reach its GitHub page and copy the url
link from your browser (eg: `https://www.github.com/username/planets`).

In your terminal, type the following commands and replace <username> by your actual GitHub user name:

```
# Move to your home directory (for Terminal.com)
cd /home

# Clone your GitHub repository locally
git clone https://www.github.com/<username>/planets

# Move to the project's folder
cd planets
```

## Git basic workflow

In this section, we will gradually introduce changes to the `Planets` project
and use git and GitHub to track and release these changes.

### Cloning the project

To get a local git version of the `Planets` project, we will clone it from
GitHub. In your terminal (from Terminal.com), type the following commands:

```
# Move to your home directory (for Terminal.com)
cd /home

# Clone the planets GitHub repository locally
git clone https://github.com/enormandeau/planets

# Move into the planets directory
cd planets
```

### Adding new files

The `planets` folder should now appear in your file browser. Since we only have
one planet, we will start by adding a second one. In the `planets/data` folder,
add a file named `Mars`. Double-click on it to open it and add a one-line
description of the planet Mars, for example:

```
Redish planet. Could this be our next destination?
```

### Editing files

In an analysis project, we would probably have to modify some code. Here, we
will modify the `planets.sh` file to display the information about the newly
added planet. Double-click on the `planet.sh` file to edit it.

In section 2 of the script, add three lines to display the name and information
about Mars. Section 2 should now look like this:

```
# Section 2 - Display the planet information
echo "Earth:"
cat data/Earth
echo

echo "Mars:"
cat data/Mars
echo
```

### Visualizing changes to project

We have added a planet in the `data` folder and modified the `planets.sh`
scripts. It is now time to use git to record these changes in our project and
share them on GitHub.

To see in what state our project is, we use:

```
git status
```

This command shows us what files have changed (*changes not staged for commit*)
or been created (*untracked changes*). We can even see the exact changes we
have made to the `planets.sh` file with the following command:

```
git diff --color
```

The lines starting with a plus sign (`+`) were just added.

### Staging (tracking) files

We now need to tell git that we want it to include this new file and the
changes to the `planets.sh` script in its history. The `git add` command can be
used to add all the changes or to add files one by one. Here, we will add both
files separately.

```
git add planets.sh
git add data/Mars
```

If we use `git status` again, we see that both files are now in a section named
*Changes to be commited*. When we commit our changes in the next section, these
files will be part of the project's history forever and we will be able to go
back to them.

### Commiting changes

To tell git to include the changes selected with `git add`, we need to commit
them with:

```
git commit -m "Add the Mars planet"
```

Commit messages are very important. They should be short and descriptive. You
need to write a message that finishes the following sentence: `When applied,
these changes will...`. Here are some examples of good commit messages:

- Fix bug with header in data
- Add new barplot figure
- Clean code of script.R
- Minor (fix typos)

### Uploading (pushing)

TODO git push

### Try adding Venus to the Solar System

Use the same steps to add the Venus planet:

- Add the `data/Venus` file
- Edit `data/Venus` to include a one line description of Venus
- Modify `planets.sh` to display the information about Venus
- Test that it is working
- Look at the project status with `git status`
- Track the changes with `git add`
- Commit the changes with `git commit -m "Add the Venus planet"`
- Upload the changes with `git push`

Congratulations! You have now mastered 90% of the important git commands.

## Visualize the project history

From time to time, you will want to look at the history of your project and
potentially go back in time. To display the history, you can use the following
command:

```
git log
```

You will need to press the `q` key to get back from the output of `git log`.

The default output of the `git log` command is not very pretty. To produce a
more useful output, use:

```
git log --oneline --color --graph --all --decorate
```

Even better, you can create an alias for this command:

```
alias gl='git log --oneline --color --graph --all --decorate'
```

Now, you can see the history by typing `gl` in the terminal.

## Time travel

TODO `git checkout`

## Interlude

At this point, you have learned about the commands that make about 90% of a
normal git workflow. It 

## Next section

In the next section, we will briefly look at a few more advanced Git
techniques.

### [05 - Advanced notions](05_advanced_notions.md)

