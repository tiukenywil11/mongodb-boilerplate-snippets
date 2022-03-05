# MongoDB count commands

## count command syntax
```bash
db.<collection>.find({
	<string_key>: '<string_value>',
	<integer_key>: <integer_value>,
	...
}).count
```

## Example working sort command
```bash
db.posts.find({ category: 'News' }).count()
```