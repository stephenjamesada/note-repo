# Configuration

If it's your first time using Git, it will, before you try to make your first commit, say `Author identity unknown`, then will tell you to run these commands:

```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

> Run these commands with the `--local` flag instead of the `--global` flag to only set these variables for your current repository.

## Commands

`git reset HEAD~`: Undoes the last commit, bringing everything back to the working directory.

`git rm <FILE>`: Deletes a file from the repository, staging that deletion at the same time. This won't work if a file has uncommitted changes, so you'd need to commit that file first and use the `--cached` flag, or `-f`/`--force` to force it to remove the file anyway. `-f` deletes it completely, `--cached` removes it only from the staging area.

`git reset --hard`: Brings back everything, including deleted files.

`git rm -r <FOLDER>`: This deletes a folder and all of its subdirectories from the repository, as the `-r` flag stands for recursive.

`git log`: Gives you an extensive history of all commits made in the repository. It shows:

- Commit ID / commit hash
- Branch where the commit was made
- Author
- Date
- Commit description

`--oneline` shows you only the ID, occasionally the commit's branch, and its description.
