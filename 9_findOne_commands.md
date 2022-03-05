# MongoDB findOne commands

## findOne command syntax
```bash
db.<collection>.findOne({ 
	<string_key>:<string_value> 
})
```

## Example working forEach command
```bash
db.posts.findOne({ 
	category : 'News' 
})
```