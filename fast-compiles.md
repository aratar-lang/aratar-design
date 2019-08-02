# Fast Compiles
The Yeet standard library aims to include the whole Yeet ecosystem.  This has failed for some programming languages, so the approach is different.

Obviously, all code can't be in the standard library - there are different approaches to the same problem.  The standard lib may support both or if one is objectively better, than the other one won't be included.  Other libraries may be imported with the `lib()` const fn.

Libs have 2 parts: memory layout (structs, enums, types), and code.

```
/compile.muon
/data/ # Data Folder (*.opus, *.png, *.txt, constants etc.)
/type/ # Type Folder (*.muon)
/code/ # Code Folder (*.code)
/libs/ # Libs Folder (*.ylib)
```

## `compile.muon`
```muon
name: mylib
type: component
      program
```
- `type`: `lib`

```yeet
# code.yeet

```
