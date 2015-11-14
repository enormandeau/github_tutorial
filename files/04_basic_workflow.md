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
cd /home/

# Clone your GitHub repository locally
git clone https://www.github.com/<username>/planets

# Move to the project's folder
cd planets
```

- Clicking the `Download ZIP` link
- Cloning project with `git clone <Project URL>`
  
## Git basic workflow

- Making some changes (adding and editing files)
- See what files have changed: `git status`
- Visualize the changes: `git diff`
- Choose files to commit `git add`
- Commit changes `git commit -m "Message"`
- Send commit to GitHub `git push`
- View log of commits with messages `git log`
  
## Differences among files and versions

- Show current uncommited changes with `git diff`
- Display history of changes with `git log`
- Better history `git log --oneline --color --graph --all --decorate`
- Create an alias for git log:

```
alias gg='echo ">>> Branches"; \
    git branch; \
    echo; \
    echo ">>> Graph"; \
    git log --oneline --color --graph --all --decorate'
```

## Using markdown in your README.md

Any `markdown` formatting you put in your README.md file will be rendered
nicely on your repository page. For example, this whole course has been created
as a repository of `markdown` files that link to each other.

Here are some basic effects:

- Use one `-` at the beginning of 2+ lines to create a list of items (like this one)
- Use `*word*` to create *italic*
- Use `**word**` to add **bold**
- Use `\`code\`` to write inline code
- Use `\`\`\`lines of code\`\`\`` to write code on multiple lines
- Use `#` `##` `###` for level 1, 2, and 3 titles
- Use `[Text](link)` to insert html links
- Use `![Text](image-location)` to insert images

## Next section
In the next section, we will briefly look at more advanced Git techniques.

### [05 - Advanced notions](05_advanced_notions.md)

