[[Bash]]
[[Terminal and Finder]]
[[Chapter 1]]

# Basic File Manipulation

We know that we can use `touch` to create new files in the current working directory, but what can we actually do to them from the terminal?

Let's say I make a typo with a `impotant-file.txt`. I can use the `mv` command (which stands for move), to rename that file, and works like `mv <TARGET> <NEW_NAME>`. Now I rename my text file with `mv impotant-file.txt important-file.txt`.

> While GUI file applications (ex. File Explorer, Finder, etc.) can stop you from making duplicates, or renaming a file that has the same name as another, the terminal does not stop you. When you do it, it overwrites the old file with new/renamed one.

