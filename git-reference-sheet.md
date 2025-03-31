#### Git Reference Sheet

```bash
### Many times it'll be just 3 simple commands:

git status
git add
git commit

# Basic Git Commands
### Initialize a new Git repository
git init

### Clone an existing repository
git clone <repository-url>

### Check the status of the repository
git status

### Add files to the staging area
git add . # `git add <file>`

# Commit changes to the repository
git commit -m "Your commit message here"  # Commit with a message

### Push changes to a remote repository
git push origin <branch-name> # Push to the specified branch (e.g., main, master)


### Others...

---

[Git Log](https://git-scm.com/docs/git-log)
# The git log command displays the commit history of a Git repository, showing information about each commit. 
# This includes the author, the date, and the commit message, providing a comprehensive view of changes over time. 
# Each commit is uniquely identified by a commit hash.

# View the commit history
git log

# This command displays the last five commits without using the pager, making it easier to view in environments where scrolling is not necessary or possible.
git --no-pager log -n 5

# This command will show the last 10 commits in the repository.
git log -n 10

# Git Log Flags

# Using --oneline to show the commit logs in a compressed single-line format:
git log --oneline
git --no-pager log --oneline

# Using --decorate with full to display commit logs with full reference names:
git log --decorate=full

# Run git log --oneline --graph --all and you should see a nice ASCII art representation of your commit history:
git log --oneline --graph --all
git --no-pager log --oneline --graph --all

# Show the commit history with a graph, oneline format, and decoration for branch names
# This command will show a graphical representation of the commit history, with each commit displayed on a single line and decorated with branch names.
git --no-pager log --oneline --decorate --graph --parents

# Git Object File Types


find .git/objects
```
