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

# Print specific row (2nd line)
```console
$bash
[bob@student-node ~]$ awk 'NR==2 {print}' sample.txt
$
```

# Print 3rd column of 2nd row
```console
$bash
[bob@student-node ~]$ awk 'NR==2 {print $3}' sample.txt
$
```

# Print line number with content
```console
$bash
[bob@student-node ~]$ awk '{print NR, $0}' sample.txt
$
```

# Print lines matching a pattern
```console
$bash
[bob@student-node ~]$ awk '/error/ {print}' sample.txt
$
```

# Filter using condition (numeric)
```console
$bash
[bob@student-node ~]$ awk '$3 > 100 {print $1}' sample.txt
$
```

# Use custom field separator (colon)
```console
$bash
[bob@student-node ~]$ awk -F: '{print $1}' /etc/passwd
$
```

# Use custom field separator (comma)
```console
$bash
[bob@student-node ~]$ awk -F, '{print $2}' file.csv
$
```
$
