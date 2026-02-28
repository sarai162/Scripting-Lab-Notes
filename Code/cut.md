# Definition: cut slices text based on delimiters or character positions.
# Use it for: pulling out fields from CSVs or system files.

# Extract 1st field using ':' delimiter
```
cut -d':' -f1 /etc/passwd
```
# Extract multiple fields
```
cut -d',' -f1,3 data.csv
```
# Extract characters 1–10
```
cut -c1-10 file.txt
```
