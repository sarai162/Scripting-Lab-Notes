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
