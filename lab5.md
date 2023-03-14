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

