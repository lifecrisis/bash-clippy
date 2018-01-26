# bash-clippy

## Introduction

This is just a fun little script I wrote that allows the user to print
a nicely-formatted quote to the standard output as if it were spoken by
Microsoft's helpful assistant, [Clippy](https://en.wikipedia.org/wiki/Office_Assistant "Office Assistant").

## Function

The `clippy` script takes a single text file argument and formats the
contents next to an ASCII art version of Clippy.  The text file must be
relatively small, otherwise formatting the text in a clean way would not be
possible.  Error messages are printed if the command is used improperly, if
the file cannot be accessed, or if the given text file is too long.

To see the script in action, use the included example text file:

```bash
# Run this command from the root of the "bash-clippy/" project directory.
./bin/clippy doc/example_quote.txt
```

You should see output similar to the following:

```
 __
 /  \   "The future remains uncertain and so it should, for it is the
 |  |   canvas upon which we paint our desires. Thus always the human
 @  @   condition faces a beautifully empty canvas. We possess only this
 || ||  moment in which to dedicate ourselves continuously to the sacred
 || ||  presence which we share and create."
 |\_/|
 \___/

```

For the curious: the quote is by author [Frank Herbert](https://en.wikipedia.org/wiki/Frank_Herbert).

## Usage

This script serves no other purpose than just being fun to use!  You can
add its output to `/etc/motd` or invoke it from some other system script
where it may brighten the day of some unsuspecting user.
