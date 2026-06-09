[[Bash]]
[[Chapter 1]]
# Terminal and Finder

The terminal uses something called a **REPL**. This stands for:

- R - *Read*
- E - *Eval*
- P - *Print*
- L - *Loop*

The terminal program runs another program, called Bash, which is your shell. The Bash shell constantly utilizes the REPL. It:

- Waits for input (Read)
- Evaluates your input (Eval)
- Prints what is there (Print)
- Waits for input again (Loop)

For example, if you run `echo "Hello world!"`, the Bash shell, in Layman terms, says:

> *"You entered the echo command. I know that command. The provided argument for the echo command is 'Hello world!'. Printing 'Hello world!' back to the user. Now I wait for more input."*

---

Bash does not exist independently, it is and must be somewhere in the system for you to use it. Specifically, it's always inside of another folder/directory, as with any other application. To check what directory it's in, run `pwd`, which stands for *Print Working Directory*.
`ls` will be able to list all contents inside of that directory.

`touch` is the command used to create a file inside of your current working directory, and `rm` is the command used to delete that file.

`clear` simply clears the terminal screen.

`cd` is the way to move in and out of directories, simply give it the name or path to the directory, and you're there.