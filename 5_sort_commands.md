# MongoDB sort commands

## sort command syntax
Putting the following values will have the following sort effect, alphabetical for string
1: ascending
-1:  descending
```bash
db.<collection>.find().sort({
	<string_key>: '<1 or -1>',
	<integer_key>: <1 or -1>,
	...
})
```

## Example working sort command
```bash
db.posts.find().sort({ title: 1 })

#To make it more readable
db.posts.find().sort({ title: 1 }).pretty()
```