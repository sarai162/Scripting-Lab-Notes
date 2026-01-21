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
