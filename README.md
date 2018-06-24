# Bash CLI input as file

> Use AWK to parse command line arguments/options from a file

## Usage example

```
./cli -h
Cli takes a file as input.
Usage: cli INPUT.txt
Input file skeleton:
foo=cats
bar=dogs
baz=mice
input=$(mktemp)
./cli -h > $input
Cli takes a file as input.
Usage: cli INPUT.txt
Input file skeleton:
cat $input
foo=cats
bar=dogs
baz=mice
./cli $input
running main...
using args:
foo is cats
bar is dogs
baz is mice
```
