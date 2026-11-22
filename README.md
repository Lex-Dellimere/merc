# merc

merc is a store for symbolic expressions, written in mettle. you load expressions, search them with patterns and run rules over them, the way MORK does, in a window or from the command line.

## build

you need the mettle compiler built from [its source](https://github.com/The-Mettle-Project/Mettle) and [mbuild](https://github.com/Lex-Dellimere/mbuild). mbuild downloads alph, MythicUI, Glint and Cryptex for you.

```
git clone https://github.com/Lex-Dellimere/merc
cd merc
mbuild build -r
```

the program is `build/linux/release/merc`. it builds and runs on linux.

## run

```
./build/linux/release/merc
```

opens the window. type `help` in the line at the bottom, or press tab on an empty line.

```
./build/linux/release/merc run program.mm2
```

runs a program of rules like `mork run` and prints what is left.

```
./build/linux/release/merc shell
```

is the same command line in a terminal.
