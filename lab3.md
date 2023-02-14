# Researching Commands

#### `grep -c "(text)" (file)`

Using `grep -c` will show the number of matches as the output. 

## Example #1
``` 
$ grep -c "the" Bahamas-Intro.txt
17
```
In this example, I use `grep -c` to count the number of "the" in `Bahamas-Intro.txt`. This command is useful because it allowed me to find the number of

```
$ grep -c "Ath3ns" Athens-WhatToDo.txt
0
``

#### `grep -n "(text)" (file)`

Using grep -n will show the line number when displaying the output. 

#### `grep -l "(text)"`

Using grep -l will display the files that contain the given string. 

#### `grep -v "(text)" (file)`

Using grep -v will invert the output and show all lines that don't match. 
