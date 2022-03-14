# MongoDB increment commands

## increment command syntax
Takes three parameters
- First parameters is supposed to ba a unique key-pair value. 
- Second would be the whole array that needs to be updated.
```bash
db.<collection>.update(
	{ 
		<id_key>:<id_value> 
	},
	{
		$inc: { 
			<integer_key>: <integer_value_increment_by_how_much>
		}
	},
)
```

## Example working increment command
```bash
db.posts.update(
	{
		title: 'Post One'
	},
	{
		$inc: {
			likes: 2
		}
	},
)
```