# Definition: xargs converts input (stdin) into command arguments.
# Use it for: applying operations to lists of files or results of find.

# Basic example
```
echo "file1 file2" | xargs rm
```
# With find
```
find . -name "*.tmp" | xargs rm
```
# Limit per command
```
cat list.txt | xargs -n 1 echo
```
# Null-safe (for filenames with spaces)
```
find . -print0 | xargs -0 rm
```
