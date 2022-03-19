# MongoDB create index commands

## create index command syntax
```bash
db.<collection>.createIndex(
	{
		<string_to_add_index>: <index_name>
	}
)
```

## Example working create index command
```bash
db.posts.createIndex(
	{
		title: 'text'
	}
)

```
