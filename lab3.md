# Researching Commands

#### `grep -c "(text)" (file)`

Using `grep -c` will show the number of matches as the output. 
Source: [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

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
Source: [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

## Example #1
``` 
$ grep -n "cafés" Cuba-WhatToDo.txt
25:Both bars and cafés are places to have a mojito, daiquiri, or shot of ron (rum), smoke a Cohiba, and — usually — hear some live Cuban rhythms. In Havana the bars not to miss are Hemingway haunts: La Bodeguita del Medio and El Floridita. Enjoyable café-bars in Havana include Café de Paris (Obispo and San Ignacio), Café O’Reilly (O’Reilly and San Ignacio), Montserrate (Avenida de Bélgica and Obrapía), and El Patio (Plaza de la Catedral). Several hotels also have good bars, including Hotel Sevilla (made famous in Graham Greene’s Our Man in Havana), Hotel Inglaterra’s rooftop bar, and Hotel Havana Libre’s Turquino (with amazing views from the 25th floor).
```
In this example, I use `grep -n` to find the line number that the phrase "cafés" appears on in `Cuba-WhatToDo.txt`. This command is useful because it allowed me to find out exactly where the text begins talking about cafés.

## Example #2
``` 
$ grep -n "fishing" Cuba-WhatToDo.txt
48:Deep-sea fishing is one of Cuba’s great attractions, though as of yet not well known (or over-fished). Trips leave from the island’s resorts and Havana’s Hemingway Marina in search of marlin, wahoo, and swordfish. Playas del Este, Varadero, and Cayo Largo are other places that offer excellent fishing expeditions. In addition, there are offshore expeditions for smaller fry such as tarpon, sea bass, and mackerel. For freshwater fishing, Hanabanilla and Zaza (near Sancti Spíritus) lakes both hold impressively big, copious large-mouth bass.
49:For information on fishing excursions, contact Puertosol (Calle Cobre, 3404, Villa Marina, Havana; Tel. 33-3510).
```
In this example, I use `grep -n` to find the line number that the phrase "fishing" appears on in `Cuba-WhatToDo.txt`. This command is useful because it allowed me to find out excatly where the text begins talking about fishing.

#### `grep -l "(text)"`

Using grep -l will display the files that contain the given string. 
Source: [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

## Example #1
``` 
$ grep -l "Greece" *
Athens-History.txt
Athens-Intro.txt
Athens-WhatToDo.txt
Athens-WhereToGo.txt
Barcelona-WhereToGo.txt
Budapest-History.txt
CostaBlanca-History.txt
Crete-History.txt
Crete-WhatToDo.txt
Crete-WhereToGo.txt
```
In this example, I use `grep -l` to find the files that mention the phrase "Greece" in `berlitz2`. This command is useful because it allowed me to find out exactly which files talk about Greece.

## Example #2
``` 
$ grep -l "climbing" *
Bali-WhatToDo.txt
Beijing-WhatToDo.txt
Berlin-WhatToDo.txt
Budapest-WhereoGo.txt
California-WhatToDo.txt
California-WhereToGo.txt
Canada-WhereToGo.txt
CanaryIslands-WhereToGo.txt
Cuba-WhereToGo.txt
Nepal-WhatToDo.txt
Nepal-WhereToGo.txt
Paris-WhereToGo.txt
Portugal-WhereToGo.txt
PuertoRico-WhereToGo.txt
Vallarta-WhereToGo.txt
```
In this example, I use `grep -l` to find the files that mention the phrase "climbing" in `berlitz2`. This command is useful because it allowed me to find out exactly which files talk about climbing.

#### `grep -v "(text)" (file)`

Using grep -v will invert the output and show all lines that don't match. 
Source: [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

## Example #1
``` 
grep -v "surfing" California-WhatToDo.txt

What to Do
Sports
Watersports
If you get no other exercise while you’re in California, it would be difficult to go without at least one day of swimming at the beach. It’s no coincidence that most of the United States’ champion swimmers come from Southern California. In the middle-class neighborhoods of Los Angeles county it seems that every other house has its own swimming pool — from the air you see the mass of turquoise blobs as you fly into the airport ...
```
In this example, I use `grep -v` to find the lines that don't mention the phrase "surfing" in `California-WhatToDo.txt` (Full output is too large to include in the code block). This command is useful because it allowed me to find out exactly which lines don't talk about surfing.

## Example #2
```
grep -v "the" China-History.txt   

A Brief History
The First Dynasty
The Chinese Empire
Under Mongol Rule
The Elegance of Ming
Pigtails and Prosperity
The Bitter Years of War
```
In this example, I use `grep -v` to find the lines that don't mention the phrase "the" in `China-History.txt`. This command is useful because it allowed me to find out exactly which lines don't use the word "the".
