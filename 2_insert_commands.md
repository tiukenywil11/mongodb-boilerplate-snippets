# MongoDB Insert commands

## Insert command syntax
- Format for the following key pair values types can be seen below.
- '...' represents being able to put more values.
```bash
db.<collection>.insert({
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

## Example working insert command
```bash
db.posts.insert({
	title: 'Post One',
	body: 'Body of post one',
	category: 'News',
	likes: 4,
	tags: ['news','events'],
	user: {
		name: 'John Doe',
		status: 'author'
	},
	date: Date()
})
```