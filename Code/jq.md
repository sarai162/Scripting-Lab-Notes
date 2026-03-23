# Definition: jq(JSON Processor) filters, transforms, and formats JSON data.
# Use it for: pretty‑printing JSON, extracting fields, and modifying config files.

## Pretty print JSON
```
jq '.' data.json
```
## Extract field
```
jq '.name' user.json
```
# Filter objects
```
jq 'select(.status=="active")' users.json
```
# Map fields
```
jq '.[] | {id, name}' users.json
```
# Update field
```
jq '.version = "2.0"' config.json
```
