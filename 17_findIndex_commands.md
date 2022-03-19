# MongoDB find using index commands

## find using index command syntax
```bash
db.<collection>.find(
	{
		$<index_name>: {
			$search: "\"<value_to_find>\"
		}
	}
)
```

## Example working find using index command
```bash
db.posts.find(
	{
		$text: {
			$search: "\"Post O\""
		}
	}
)

# To make it more readable

db.posts.find(
	{
		$text: {
			$search: "\" Post O\""
		}
	}
).pretty 
```
