# MongoDB rename commands

## rename command syntax
Takes two parameters
- First parameters is supposed to ba a unique key-pair value. 
- Second would be the whole array that needs to be renamed.
```bash
db.<collection>.update(
	{ 
		<id_key>:<id_value> 
	},
	{
		$rename: { 
			<to_be_replaced_key>: <replace_with_this_key>
		}
	},
)
```

## Example working rename command
```bash
db.posts.update(
	{
		title: 'Post One'
	},
	{
		$rename: {
			likes: 'views'
		}
	},
)
```