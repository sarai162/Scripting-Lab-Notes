# By default sed prints 2 times (1 time for the unprocessed output and 1 time for the processed output)

## Example terminal session

```console
$ bash 
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
