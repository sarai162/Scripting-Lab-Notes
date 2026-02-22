# Definition: grep searches files or input for lines matching a pattern.
# Use it for: filtering logs, pattern matching, and quick text search.

# Examples

# Basic search
```
grep "error" file.txt
```
# Case-insensitive
```
grep -i "error" file.txt
```
# Recursive search
```
grep -R "TODO" .
```
# Show line numbers
```
grep -n "main" app.c
```
# Only filenames with matches
```
grep -l "config" -R .
```
# Only the matched part
```
grep -o "cat" animals.txt
```
