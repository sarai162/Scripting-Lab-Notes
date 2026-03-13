# Definition: uniq filters repeated lines from sorted input.
# Use it for: deduplication, frequency counts, and data cleanup.

# Remove duplicates (requires sorted input)
```
uniq sorted.txt
```
# Count occurrences
```
uniq -c sorted.txt
```
# Show only duplicates
```
uniq -d sorted.txt
```
