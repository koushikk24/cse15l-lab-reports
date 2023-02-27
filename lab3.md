# Researching Commands

#### `grep -c "(text)" (file)`

Using `grep -c` will show the number of matches as the output. 
Source: [[Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

## Example #1
``` 
$ grep -c "very" Bahamas-Intro.txt
4
```
In this example, I use `grep -c` to count the number of times that the phrase "very" appears in `Bahamas-Intro.txt`. This command is useful because it helped me find whether or not the phrase "very" occurs many times in the given text. 

## Example #2
```
$ grep -c "Parthenon" Athens-WhatToDo.txt
1
```
In this example, I use `grep -c` to count the number of times that the phrase "Parthenon" appears in `Athens-WhatToDo.txt`. This command is useful because it allowed me to find out whether or not the given text mentioned the Parthenon.

#### `grep -n "(text)" (file)`

Using grep -n will show the line number when displaying the output. 
Source: [[Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

## Example #1
``` 
$ grep -n "cafés" Cuba-WhatToDo.txt
25:Both bars and cafés are places to have a mojito, daiquiri, or shot of ron (rum), smoke a Cohiba, and — usually — hear some live Cuban rhythms. In Havana the bars not to miss are Hemingway haunts: La Bodeguita del Medio and El Floridita. Enjoyable café-bars in Havana include Café de Paris (Obispo and San Ignacio), Café O’Reilly (O’Reilly and San Ignacio), Montserrate (Avenida de Bélgica and Obrapía), and El Patio (Plaza de la Catedral). Several hotels also have good bars, including Hotel Sevilla (made famous in Graham Greene’s Our Man in Havana), Hotel Inglaterra’s rooftop bar, and Hotel Havana Libre’s Turquino (with amazing views from the 25th floor).
```
In this example, I use `grep -n` to find the line number that the phrase "cafés" appears on in `Cuba-WhatToDo.txt`. This command is useful because it allowed me to find out where the text begins talking about cafés.

## Example #2
``` 
$ grep -n "cafés" Cuba-WhatToDo.txt
25:Both bars and cafés are places to have a mojito, daiquiri, or shot of ron (rum), smoke a Cohiba, and — usually — hear some live Cuban rhythms. In Havana the bars not to miss are Hemingway haunts: La Bodeguita del Medio and El Floridita. Enjoyable café-bars in Havana include Café de Paris (Obispo and San Ignacio), Café O’Reilly (O’Reilly and San Ignacio), Montserrate (Avenida de Bélgica and Obrapía), and El Patio (Plaza de la Catedral). Several hotels also have good bars, including Hotel Sevilla (made famous in Graham Greene’s Our Man in Havana), Hotel Inglaterra’s rooftop bar, and Hotel Havana Libre’s Turquino (with amazing views from the 25th floor).
```
In this example, I use `grep -n` to find the line number that the phrase "cafés" appears on in `Cuba-WhatToDo.txt`. This command is useful because it allowed me to find out where the text begins talking about cafés.

#### `grep -l "(text)"`

Using grep -l will display the files that contain the given string. 
Source: [[Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

#### `grep -v "(text)" (file)`

Using grep -v will invert the output and show all lines that don't match. 
Source: [[Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
