# Printing multiple lines using awk command
```console
$bash
[bob@student-node ~]$ cat lines.txt
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
[bob@student-node ~]$ awk '{ print "Hello" }' lines.txt
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
$
```

# Printing single line 
```console
$bash
[bob@student-node ~]$ awk 'END { print "Hello" }' lines.txt
Hello
$
```

# Print entire file
```console
$bash
[bob@student-node ~]$ awk '{print}' sample.txt
$
```

# Print specific column (1st column)
```console
$bash
[bob@student-node ~]$ awk '{print $1}' sample.txt
$
```

# Print multiple columns
```console
$bash
[bob@student-node ~]$ awk '{print $1, $3}' sample.txt
$
```

