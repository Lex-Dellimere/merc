# merc

merc is a store for symbolic expressions, written in mettle. you load expressions, search them with patterns and run rules over them, the way MORK does, in a window or from the command line.

## build

you need the mettle compiler built from [its source](https://github.com/The-Mettle-Project/Mettle) and [mbuild](https://github.com/Lex-Dellimere/mbuild). merc also needs alph, MythicUI, Glint and Cryptex in a folder named `mettle` next to it:

```
git clone https://github.com/Lex-Dellimere/merc
mkdir mettle
git clone https://github.com/Lex-Dellimere/Alph mettle/alph
git clone https://github.com/Lex-Dellimere/MythicUI mettle/mythic_ui
git clone https://github.com/Lex-Dellimere/Glint mettle/glint
git clone https://github.com/Lex-Dellimere/Cryptex mettle/cryptex
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
