[[Git]]
# Git Architecture

***What is a Git repository?*** a Git repository is any place where you want Git to host your project. To create one, you execute the following commands:

```bash
mkdir -p project
cd project
git init
```

`git init` is what creates the repository in your folder, and tells git to initialize the repository in your current working directory, given that's what init means here. It creates a `.git` subdirectory in your project folder, which contains everything Git needs to track your project properly, among other things, such as:

- Changes made
- Who made those changes
- Previous versions of those files

Seeing the `.git` dotfile present in a directory almost certainly tells you that the directory is a Git repository.

---

A remote repository stores and hosts your local files elsewhere for easier access and portability. GitHub is used for this. To do this, go to GitHub, create an account if you haven't, and go to `Top Repositories > New` on the homepage. Then, you will:

1. Give your repository a name and description
2. Create

> GitHub gives you other options for repository configuration such as visibility toggling (public/private), adding a `README.md`, `.gitignore`, or license (shown in the repo as `LICENSE` when used).

To add to this new GitHub repository, create a new file there or upload your own. GitHub has a text editor inside when you need to edit a file, useful for small/quick changes. On the same page you're using the web-based editor, there is a *Commit changes...* button that allows you to commit the changes you've made to that exact file, with a message and optional extended description.

A local repository is a repository that is on your machine only, while a remote repository is a repository that is hosted elsewhere, but can be present on both your machine and where it is held in the cloud. 

To bring a remote repository down to your machine, you use the `git clone` command. Syntax:

`git clone https://github.com/[repo_creator]/[repo_name].git`

If you don't know one of, or either of those names, you can grab the link from the green *Code* button when you view your repository. Your repo will be cloned into your current working directory.

---

## Other Commands

`git status`: Tracks changes that are either staged or unstaged, and shows the modified files, giving a tight and concise summary of the current state of work being done to what's inside of the repository.

`git add`: Adds, or *stages* any files in your working directory that you specify to the staging area. `git add .` stages all changes within the current directory and everything in it, including subdirectories. For example, `git add README.md` only stages a README and its changes, and nothing else. `git add --all` or `-A` accounts for the entire repo. `git add *` stages every change visible, excluding deleted ones. Can stage by file extension as well via wildcard (`*.txt`).

`git reset`: Resets the staging area, so everything that was staged before this command was run is now unstaged, and does not touch your working directory. When executed, it shows you all unstaged changes after the reset.

`git commit`: Tells Git to save all staged changes permanently. The `-m` flag stands for message, used to give a description for your changes. For example `git commit -m "Removed semantic content from document.txt and replaced with overall summary"`.