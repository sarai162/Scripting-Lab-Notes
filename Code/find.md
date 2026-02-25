# Definition: find locates files/directories based on name, size, date, and more.
# Use it for: scanning directory trees and automating cleanups.

# Examples

# Find by name
```
find . -name "*.txt"
```
# Find by type (f = file, d = directory)
```
find . -type f -name "*.log"
```
# Find by size
```
find . -size +10M
```
# Find and delete
```
find . -name "*.tmp" -delete
```
# Run command on results
```
find . -name "*.log" -exec wc -l {} \;
```
# Find modified in last 1 day
```
find . -mtime -1
```
