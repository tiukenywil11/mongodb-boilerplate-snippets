# MongoDB remove commands

## remove command syntax
```bash
db.<collection>.remove(
	{ 
		<id_key>:<id_value> 
	}
)
```

## Example working remove command
```bash
db.posts.remove(
	{
		title: 'Post Four'
	}
)
```