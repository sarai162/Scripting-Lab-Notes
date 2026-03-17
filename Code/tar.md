# Definition: tar bundles files/folders into archives, optionally compressed.
# Use it for: backups, packaging projects, and transferring folders.

# Create tar archive
```
tar -cvf archive.tar folder/
```
# Extract tar archive
```
tar -xvf archive.tar
```
# Create gzip-compressed archive
```
tar -czvf archive.tar.gz folder/
```
# Extract gzip archive
```
tar -xzvf archive.tar.gz
```
# List contents
```
tar -tf archive.tar.gz
```
