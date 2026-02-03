# By default sed prints 2 times (1 time for the unprocessed output and 1 time for the processed output)

## Example terminal session

```console
$bash 
[bob@student-node ~]$ sed 'p' <<< "Hello"
Hello
Hello
$
```

# The -n flag helps resolve this by only printing the processed output to the terminal

```console
$bash
[bob@student-node ~]$ sed -n 'p' <<< "Hello"
Hello
$
```
# Printing even lines in sed 

```console
$bash
[bob@student-node ~]$ sed -n 'n;p' lines.txt
2
4
6
8
10
12
14
$
```

# Printing odd lines in sed

```console
$bash
[bob@student-node ~]$ sed -n 'p;n' lines.txt
1
3
5
7
9
11
13
15
$
```

# Print entire file 

```console
$bash
[bob@student-node ~]$ sed '' sample.txt
$
```

# Print specific line (3rd line)

```console
$bash
[bob@student-node ~]$ sed -n '3p' sample.txt
$
```

# Print range of lines (1 to 5)
```console
$bash
[bob@student-node ~]$ sed -n '1,5p' sample.txt
$
```

# Search and print matching lines

```console
$bash
[bob@student-node ~]$ sed -n '/error/p' sample.txt
$
```

# Delete a specific line

```console
$bash
[bob@student-node ~]$ sed '3d' sample.txt
$
```

# Delete a range of lines

```console
$bash
[bob@student-node ~]$ sed '1,5d' sample.txt
$
```

# Delete lines matching a pattern

```console
$bash
[bob@student-node ~]$ sed '/error/d' sample.txt
$
```

# Replace first occurrence in each line

```console
$bash
[bob@student-node ~]$ sed 's/old/new/' sample.txt
$

```

# Replace all occurrences in each line

```console
$bash
[bob@student-node ~]$ sed 's/old/new/g' sample.txt
$
```

# Replace text and edit file in place

```console
$bash
[bob@student-node ~]$ sed -i 's/old/new/g' sample.txt
$
```

# More examples 

```console
$bash

# Insert line before a matching pattern
[bob@student-node ~]$ sed '/error/i This line is inserted' sample.txt

# Append line after a matching pattern
[bob@student-node ~]$ sed '/error/a This line is appended' sample.txt

# Change (replace) entire matching line
[bob@student-node ~]$ sed '/error/c This line is replaced' sample.txt

# Case-insensitive search and print
[bob@student-node ~]$ sed -n '/error/Ip' sample.txt

# Use alternate delimiter (avoid slash conflict)
[bob@student-node ~]$ sed 's|/usr/bin|/bin|g' sample.txt

$
```
