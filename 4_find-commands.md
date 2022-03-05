# MongoDB find commands

## Find command syntax
```bash
db.<collection>.find({
	<string_key>: '<string_value>',
	<integer_key>: <integer_value>,
	<array_key>: ['<array_value1>','<array_value2>',...],
	<object_key>: {
		<inner_string_object_key1>: '<inner_string_object_value>',
		...
	},
	date: Date()
	...
})
```

## Example working find command
```bash
db.posts.find({ category: 'News' })
```