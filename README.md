# CITS3403: Git Basics

- Install <b>Git</b> and <b>Git Bash</b> (Windows) or install Git standalone (Mac) from the following link: https://git-scm.com/downloads. Alternatively if you have Homebrew, run the command `brew install git`.

- Start by forking this repository on GitHub using the `Fork` button and selecting your account.

<img src='src/fork.jpg'></img>

- Go to your newly created repository (should be visitable via `https://www.github.com/your-username-here/learn-git`) and `Clone` the repository by copying the link (https://github.com/1997/learn-git.git) or copying to clipboard.

<img src='src/clone.jpg'></img>

Navigate to a place on your computer to store the repository, and run the command `git clone https://github.com/1997/learn-git.git`.

- Fetch all remote branches by running `git fetch`.

- Set up your email and account name by using `git config --global user.name "Your Name Here"` and `git config --global user.email email@email.com`.

# Exercises

## Creating a new Branch

- Create a new branch and navigate to it using the `git checkout -b <branchname>` command.

## Committing and Pushing Changes

- Open `main.py`, and change `Hello World` in the `print_string()` function to `Git Changes`. Save your change.

- On command line, run `git status` to check your current status. `main.py` should be modified.

- <b>Commit</b> these changes by adding the files you want to commit: 
`git add <filename>` or `git add .` for all files. Commit these files using the `git commit -m"Commit Message Here"` command.

- <b>Push</b> these changes to your own remote repository.
`git push origin <your new branch name>`

## Creating a Pull Request

Create a Pull Request by visiting GitHub and pick your new branch to merge into `master`.

# Helpful Tips

- Name your branches accordingly. If you are fixing a specific issue, label it `<specific issue>-bug`. Alternatively, if you use <b>Trello</b>, <b>Jira</b> or <b>GitHub Actions</b>, you can name the branches card numbers or reference numbers.

- Create <b>GitHub Issues</b> and a project board to keep organised with tasks and your agile sprints.

- Every time you begin work on your project, run `git pull origin <branchname>` to pull from the higher remote node, making sure that changes that were added to the higher node by other people are synchronised into your work, avoiding merge conflicts.
