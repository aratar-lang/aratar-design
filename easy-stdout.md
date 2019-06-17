# Easy Stdout
In order to allow usage by the REPL as a calculator, simple expressions shall print out their evalutation to stdout.

## Examples
```
(2 + 3) - 1         # Integer
"Hello, world"      # String
1.5 - 1.0           # Fixed point
{4 1.0} + {2 0.5}   # Tuple addition
{1 2} + {3 4}       # Vector addition
[1 2] [3 4]         # Append list
[1 2] + [3 4]       # List addition
0x11 + 0xF1         # Hexadecimal addition
0b1 + 0b11          # Binary addition
0o4 + 0o4           # Octal addition
```

> 4
> Hello, world
> 0.5
> {6, 1.5}
> {4 6}
> \[1 2 3 4\]
> \[4 6\]
> 0x102
> 0b100
> 0o10
