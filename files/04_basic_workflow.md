# Basic Workflow

## Creating a new project

Normally, you would have to create a new project. But,now that you have an
active project, `Planets`, to work with, we will download it on your computer
to work on it.

## Using the Git basic workflow

In this section, we will gradually introduce changes to the `Planets` project
and use Git and GitHub to track and release these changes.

### Cloning the project

To get a local Git version of the `Planets` project, we will clone it from
GitHub. In your terminal, type the following commands and
replace `<username>` by your GitHub user name:

```bash
# Move to your home directory
cd /home # or cd /Users on Mac

# Clone the planets GitHub repository locally
git clone https://github.com/<username>/planets

# Move into the planets directory
cd planets
```

### Adding new files

The `planets` folder should now appear in your file browser. Since we only have
one planet, we will start by adding a second one. In the `planets/data` folder,
add a file named `Mars`. Double-click on it to open it and add a one-line
description of the planet Mars, for example:

```bash
Reddish planet. Could this be our next destination?
```

### Editing files

In an analysis project, we would probably have to modify some code. Here, we
will modify the `planets.sh` file to display the information about the newly
added planet. Double-click on the `planet.sh` file to edit it.

In section 2 of the script, add three lines to display the name and information
about Mars. Section 2 should now look like this:

```bash
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
scripts. It is now time to use Git to record these changes in our project and
share them on GitHub.

To see in what state our project is, we use:

```bash
git status
```

This command shows us what files have changed (*changes not staged for commit*)
or been created (*untracked changes*). We can even see the exact changes we
have made to the `planets.sh` file with the following command:

```bash
git diff --color
```

The lines starting with a plus sign (`+`) were just added.

### Staging (tracking) files

We now need to tell Git that we want it to include this new file and the
changes to the `planets.sh` script in its history. The `git add` command can be
used to add all the changes or to add files one by one. Here, we will add both
files separately.

```bash
git add planets.sh
git add data/Mars
```

If we use `git status` again, we see that both files are now in a section named
*Changes to be commited*. When we commit our changes in the next section, these
files will be part of the project's history forever and we will be able to go
back to them.

### Commiting changes

To tell Git to include the changes selected with `git add`, we need to commit
them with:

```bash
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

All is now ready for us to send our changes online on GitHub.

```bash
git push
```

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

Congratulations! You have now mastered 90% of the important Git commands.

## Visualizing the project history

From time to time, you will want to look at the history of your project and
potentially go back in time. To display the history, you can use the following
command:

```bash
git log
```

You will need to press the `q` key to get back from the output of `git log`.

The default output of the `git log` command is not very pretty. To produce a
more useful output, use:

```bash
git log --oneline --graph --decorate
```

Even better, you can create an alias for this command:

```bash
alias gl='git log --oneline --graph --decorate'
```

Now, you can see the history by typing `gl` in the terminal.

## Time travel

We can use the `git checkout` command to go back to previous states of our
project. When you use the `git log --oneline --graph --decorate` command,
a seven character identifier is shown near the begining of the line. We can
use these identifiers to move back and forward in time. Try it with the
following command and change `<commit-id>` by the identifier shown by `git log`.

```bash
git checkout <commit-id>
```

Use `git log --oneline --graph --decorate` again to see that you have moved.
The `HEAD` identifier indicates where in history we are currently situated. To
move back to the most recent commit, you can either use its commit ID or use
`master`. For example, you can use:

```bash
git checkout master
```

You are now at the most recent commit.

## Next section

In the next section, we will briefly look at a few more advanced Git
techniques.

### [05 - Advanced notions](05_advanced_notions.md)

