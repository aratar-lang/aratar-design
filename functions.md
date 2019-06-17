# Built-In Functions
There shall be no difference in Yeet, between keywords and standard library functions.  They both are implemented as functions.  Exported functions begin with a capital letter.

## Functions

### `fn par`
Dequeue a parameter from the function.
* `type: type` - The type of the parameter to grab.
```
#################
## Entry Point ##
#################

# Run `myfunction` to generate a message.
Let message:
    myfunction
        a: "Hello, world!"
        b: 75
# Print out the message we got.
message

###############
## Functions ##
###############

Def myfunction:
    ### Documentation for `myfunction`.
    # Parse parameters
    Let a: Par @Text        ### First parameter documentation.
    Let b: Par Int 0~100    ### Second parameter documentation.
    # Print out text and number on one line.
    Out message: Text a ' ' b '.'
:myfunction
```

### `fn let`

### `fn var`

### `fn out`
