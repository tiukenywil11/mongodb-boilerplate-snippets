# MongoDB Insert many commands

## Insert many command syntax
- Format for the following key pair values types can be seen below.
- '...' represents being able to put more values.
```bash
db.<collection>.insert([
	{
		<string_key>: '<string_value>',
		<integer_key>: <integer_value>,
		<array_key>: ['<array_value1>','<array_value2>',...],
		<object_key>: {
			<inner_string_object_key1>: '<inner_string_object_value>',
			...
		},
		date: Date()
		...
	},
	{
		<string_key>: '<string_value>',
		<integer_key>: <integer_value>,
		<array_key>: ['<array_value1>','<array_value2>',...],
		<object_key>: {
			<inner_string_object_key1>: '<inner_string_object_value>',
			...
		},
		date: Date()
		...
	},
	{
		<string_key>: '<string_value>',
		<integer_key>: <integer_value>,
		<array_key>: ['<array_value1>','<array_value2>',...],
		<object_key>: {
			<inner_string_object_key1>: '<inner_string_object_value>',
			...
		},
		date: Date()
		...
	},
	...
])
```

## Example working insert many command
```bash
db.posts.insertMany([
	{
		title: 'Post Two',
		body: 'Body of post two',
		category: 'Technology',
		date: Date()
	},
	{
		title: 'Post Three',
		body: 'Body of post three',
		category: 'Technology',
		date: Date()
	},
	{
		title: 'Post Four',
		body: 'Body of post four',
		category: 'Enteratainment',
		date: Date()
	}
])


```