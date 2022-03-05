# MongoDB updateOne commands

## update command syntax
Takes three parameters
- First parameters is supposed to ba a unique key-pair value. 
- Second would be the whole array that needs to be updated.
- Third would be options (e.g. upsert: will create a new entry if not found)
```bash
db.<collection>.update(
	{ 
		<id_key>:<id_value> 
	},
	{
		$set: {
			<string_key>: '<string_value>',
			<integer_key>: <integer_value>,
			<array_key>: ['<array_value1>','<array_value2>',...],
			<object_key>: {
				<inner_string_object_key1>: '<inner_string_object_value>',
				...
			},
			date: Date()
			...
		}
	},
	{
		<option_key>: <option_value>
	}
)
```

## Example working update command
```bash
db.posts.update(
	{
		title: 'Post Two'
	},
	{
		$set: {
			title: 'Post Two',
			body: 'New post 2 body',
			date: Date()
		}
	},
	{
		upsert: true
	}
)
```