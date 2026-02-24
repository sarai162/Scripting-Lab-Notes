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
