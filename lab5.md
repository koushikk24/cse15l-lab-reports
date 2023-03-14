# Researching Commands Pt 2

#### `find (dir) -name (file)`

Using `find -name` allows the find command to search by file name. Source: [https://www.geeksforgeeks.org/find-command-in-linux-with-examples/](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

## Example #1
````
find ./ -name Budapest-WhereoGo.txt
.//Budapest-WhereoGo.txt
````
In this example, I use `find -name` to find the path to the file `Budapest-WhereoGo.txt`.

## Example #2
````
find ./berlitz2 -name Canada-History.txt
./berlitz2/Canada-History.txt
````
In this example, I use `find -name` to find the path to the file `Canada-History.txt` in the directory `berlitz2`.

#### `find (dir) -empty`
Using `find -empty` allows the find command to search for empty files and directories. Source: [https://www.geeksforgeeks.org/find-command-in-linux-with-examples/](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

## Example #1
````
find ./berlitz2 -empty

````
In this example, I use `find -empty` to find the path to all the empty files and directories in `berlitz2`.

## Example #2
````
find ./travel_guides -empty
./travel_guides/test
````
In this example, I use `find -empty` to find the path to all the empty files and directories in `travel_guides`.

#### `find (dir) -perm (permission)`
Using `find -perm` allows the find command to search for all directories with the given permissions. Source: [https://www.geeksforgeeks.org/find-command-in-linux-with-examples/](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

## Example #1
````
find ./travel_guides -perm 644
./travel_guides/.DS_Store
````
In this example, I use `find -perm` to find the path to all the directories with read/write permissions in `travel_guides`.

## Example #2
````
find ./berlitz2 -perm 644

````
In this example, I use `find -perm` to find the path to all the directories with read/write permissions in `berlitz2`.

#### `find (dir) -ctime (time)`
Using `find -ctime` allows the find command to search for all files and directories created/modified in a given time period. Source: [https://stackoverflow.com/questions/5893748/linux-command-to-check-new-files-in-file-system](https://stackoverflow.com/questions/5893748/linux-command-to-check-new-files-in-file-system)

## Example #1
````
find ./ -ctime +0  -ctime -45
./
.//Portugal-History.txt
.//Berlin-WhereToGo.txt
.//Costa-History.txt
.//Amsterdam-WhereToGo.txt
.//Costa-WhereToGo.txt
.//Amsterdam-WhatToDo.txt
.//CostaBlanca-WhatToDo.txt
.//Barcelona-History.txt
.//Portugal-WhereToGo.txt
.//Boston-WhereToGo.txt
.//Poland-WhatToDo.txt
.//California-WhereToGo.txt
.//Cuba-WhatToDo.txt
.//Berlin-History.txt
.//Bahamas-WhereToGo.txt
.//Cancun-WhatToDo.txt
.//Bali-History.txt
.//Crete-WhereToGo.txt
.//Athens-History.txt
.//Berlin-WhatToDo.txt
.//Canada-WhereToGo.txt
.//Bali-WhereToGo.txt
.//Budapest-WhereoGo.txt
.//Barcelona-WhereToGo.txt
.//Athens-WhereToGo.txt
.//Paris-WhereToGo.txt
.//China-WhereToGo.txt
.//Bermuda-WhatToDo.txt
.//California-History.txt
.//Vallarta-History.txt
.//Budapest-WhatToDo.txt
.//Cancun-History.txt
.//PuertoRico-WhatToDo.txt
.//Vallarta-WhatToDo.txt
.//Bali-WhatToDo.txt
.//CostaBlanca-History.txt
.//CstaBlanca-WhereToGo.txt
.//NewOrleans-History.txt
.//PuertoRico-History.txt
.//Algarve-Intro.txt
.//Nepal-History.txt
.//China-History.txt
.//Canada-History.txt
.//Crete-History.txt
.//Portugal-WhatToDo.txt
.//Bahamas-Intro.txt
.//Amsterdam-History.txt
.//Bahamas-WhatToDo.txt
.//Barcelona-WhatToDo.txt
.//Algarve-WhatToDo.txt
.//PuertoRico-WhereToGo.txt
.//Cuba-WhereToGo.txt
.//Costa-WhatToDo.txt
.//Beijing-History.txt
.//Nepal-WhereToGo.txt
.//CanaryIslands-WhereToGo.txt
.//Bermuda-history.txt
.//CanaryIslands-History.txt
.//Amsterdam-Intro.txt
.//Crete-WhatToDo.txt
.//Algarve-WhereToGo.txt
.//Athens-Intro.txt
.//Algarve-History.txt
.//Poland-History.txt
.//Beijing-WhereToGo.txt
.//CanaryIslands-WhatToDo.txt
.//California-WhatToDo.txt
.//Budapest-History.txt
.//China-WhatToDo.txt
.//Athens-WhatToDo.txt
.//Nepal-WhatToDo.txt
.//Bermuda-WhereToGo.txt
.//Paris-WhatToDo.txt
.//Cuba-History.txt
.//Vallarta-WhereToGo.txt
.//Bahamas-History.txt
.//Beijing-WhatToDo.txt
.//Cancun-WhereToGo.txt
````
In this example, I use `find -ctime` to find the paths to all the files and directories that were created/modified in the past 45 days in `berlitz2`.

## Example #2
````
find ./ -ctime +0  -ctime -10

````
In this example, I use `find -ctime` to find the paths to all the files and directories that were created/modified in the past 10 days in `berlitz2`.

