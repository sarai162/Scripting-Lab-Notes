# Definition: tr translates, replaces, compresses, or removes characters.
# Use it for: case conversion, cleanup, and formatting text streams.

# Convert lowercase to uppercase
```
tr 'a-z' 'A-Z' < file.txt
```
# Delete digits
```
tr -d '0-9' < file.txt
```
# Replace spaces with newlines
```
tr ' ' '\n' < words.txt
```
