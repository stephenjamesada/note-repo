# Repository

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