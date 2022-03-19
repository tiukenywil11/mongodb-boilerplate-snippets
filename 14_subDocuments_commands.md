# MongoDB sub documents commands

## sub documents command syntax
Takes two parameters
- First parameters is supposed to ba a unique key-pair value. 
- Second would be the array that needs sub documents to be added. 
```bash
db.<collection>.update(
	{ 
		<id_key>:<id_value> 
	},
	{
		$set: { 
			<sub_document_name>: [
				{
					<string_key>: '<string_value>',
					...
				},
				{
					<string_key>: '<string_value>',
					...
				}
				...
			]
		}
	}
)
```

## Example working sub documents command
```bash
db.posts.update(
	{
		title: 'Post One'
	},
	{
		$set: {
			comments: [
				{
					user: 'Mary Williams',
					body: 'Comment One',
					date: Date()
				},
				{
					user: 'Harry White',
					body: 'Comment Two',
					date: Date()
				}
			]
		}
	}
)
```