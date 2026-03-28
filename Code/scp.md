# Definition: scp(Secure Copy Protocol) copies files over SSH securely.
# Use it for: transferring files to/from remote hosts.

# Copy a file to server
```
scp file.txt user@server:/tmp/
```
# Copy directory recursively
```
scp -r project/ user@server:/var/www/
```
# Copy file from server
```
scp user@server:/etc/config .
```
