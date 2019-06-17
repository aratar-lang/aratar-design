# Domain Specific Languages
This is a way to define a mini programming language within Yeet.  See [Rust](https://doc.rust-lang.org/stable/rust-by-example/macros/dsl.html).

## Commands as a language
We should support running commands similar to how bash does.  Let's look at a bash command:

```
ls -aR -1
```

Usually, this will look for `ls` in any of the folders in your `$PATH`, and then everything else is separated by spaces, and passed as arguments (parameters) to your program.  These parameters are then parsed by the program `ls`, and the parameters only have this meaning for `ls`.  Of course there is some things that are common between unix commands, but the programmers of `ls` aren't forced to follow them if it doesn't work for their use case.

In Yeet, keywords and functions shall work like bash commands.  For instance, let's define a function:

```
Def myfunction:
    ### Documentation for `myfunction`.
    # Parse parameters
    Let a: Par @Text        ### First parameter documentation.
    Let b: Par Int 0~100    ### Second parameter documentation.
    # Print out text and number on one line.
    Out message: Text a ' ' b '.'

Def myfunction
### A function that does nothing.

Def myfunction:
### A function that prints "Hello, world 5!"
    Let a: 2 + 3
    "Hello, world $a!"
```
