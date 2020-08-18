# How to Use Command Line Arguments

Extended tutorial: [Stack Abuse](https://stackabuse.com/command-line-arguments-in-node-js/).

## Passing the arguments to the program

When running an application through the command line interface (CLI), you can pass arguments by adding them after the program/script name in your prompt, separating each argument by a space, just like the following:

`$ [runtime] [script_name] [argument-1 argument-2 argument-3 ... argument-n]`

Runtime can be anything that executes a program/script e.g. sh, java, node, etc. 

## Retrieving the arguments inside the program

After you had passed the arguments while calling the program, you can access them with the  `process.argv` array.

This array will contain the interpreter and file names on the indexes 0 and 1, respectively, and all the following arguments starting from index 2. You can access your arguments by using the index number just as you do with any array.

An alternative is to create a new array by using `process.argv.slice(2)`. This new array will contain only the passed arguments.