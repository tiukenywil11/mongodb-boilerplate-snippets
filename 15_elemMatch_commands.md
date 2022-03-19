# MongoDB find using sub documents commands

## find using sub documents command syntax
Takes two parameters
- First parameters is supposed to ba a unique key-pair value. 
- Second would be the array that needs sub documents to be added. 
```bash
db.<collection>.find(
	{ 
		<sub_document_name>: {
			$elemMatch: {
				<string_key>: '<string_value>'
				...
			}
		}
	}
)
```

## Example working find using sub documents command
```bash
db.posts.find(
	{
		comments: {
			$elemMatch: {
				user: 'Mary Williams'
			}
		}
	}
)

#To make it more readable

db.posts.find(
	{
		comments: {
			$elemMatch: {
				user: 'Mary Williams'
			}
		}
	}
).pretty()

```
