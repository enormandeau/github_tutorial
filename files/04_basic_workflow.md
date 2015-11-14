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

### Adding new files

TODO add data/mars and fill it

### Editing files

TODO edit `planets.sh` to display mars

### Visualizing changes to project

TODO git status
TODO git diff

### Staging (tracking) files

TODO git add

### Commiting changes

TODO git commit -m ""

### Uploading (pushing)

TODO git push

### Once again, with Venus

Use the same steps to add the planet venus:

- Add the file `data/venus`
- Edit `data/venus` to include a one line description of venus
- Modify `planets.sh` to display venus
- Test that it is working
- Look at the project status with `git status`
- Track the changes with `git add`
- Commit the changes with `git commit -m "Add venus"`
- Upload the changes with `git push`

Congratulations! You have now mastered 90% of the important git commands.
  
## Visualize the project history

From time to time, you will want to look at the history of your project and
potentially go back in time. To display the history, you can use the following
command:

```
git log
```

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

## Differences among files and versions

- Show current non committed changes with `git diff`

## Using markdown in your README.md

Any `markdown` formatting you put in your README.md file will be rendered
nicely on your GitHub repository page. For example, this whole course has been
created as a repository of `markdown` files that link to each other.

Here are some basic effects that you can add to markdown files:

- Use one `-` at the beginning of 2+ lines to create a list of items (like this one)
- Use `*word*` to create *italic*
- Use `**word**` to add **bold**
- Use <code>\`code\`</code> to write inline code
- Use `\`\`\`lines of code\`\`\`` to write code on multiple lines
- Use `#` `##` `###` for level 1, 2, and 3 titles
- Use `[Text](link)` to insert html links
- Use `![Text](image-location)` to insert images
- Since markdown is translated into HTML, you can use HTML in your files

## Next section
In the next section, we will briefly look at more advanced Git techniques.

### [05 - Advanced notions](05_advanced_notions.md)

