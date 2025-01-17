## flags

### Instructions

Write a **program** that can take `--insert` (or `-i`), `--order` (or `-o`) and a `string` as arguments.

This program should :

- Insert the string given to the `--insert` (or `-i`), into the argument `string`, if given.
- If the flag `--order` (or `-o`) is given, order the `string` argument (in ASCII order).
- If there are no arguments or if the flag `--help` (or `-h`) is given, the options should be printed as in the example.

Example of output :

```console
$ go run . --insert=4321 --order asdad
1234aadds
$ go run . --insert=4321 asdad
asdad4321
$ go run . asdad
asdad
$ go run . --order 43a21
1234a
$ go run .
--insert
  -i
    This flag inserts the string into the string passed as argument.
--order
  -o
    This flag will behave like a boolean, if it is called it will order the argument.
$
$ go run . -h
--insert
  -i
    This flag inserts the string into the string passed as argument.
--order
  -o
    This flag will behave like a boolean, if it is called it will order the argument.
$
$ go run . --help
--insert
  -i
    This flag inserts the string into the string passed as argument.
--order
  -o
    This flag will behave like a boolean, if it is called it will order the argument.
$
```
