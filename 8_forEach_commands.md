# MongoDB forEach commands

## forEach command syntax
forEach takes in a function
```bash
db.<collection>.find().forEach(
	function(<parameter>) 
	{
		<commands>
	}
)
```

## Example working forEach command
```bash
db.posts.find().forEach(
	function(doc) 
	{
		print('Blog Post: ' + ' doc.title')
	}
)

```