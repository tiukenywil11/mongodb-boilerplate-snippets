# MongoDB conditionals commands

## conditionals command syntax
```bash
# greater than
db.<collection>.find(
	{
		<interger_key>: {
			$gt: <integer>
		}
	}
)

# greater than equals
db.<collection>.find(
	{
		<interger_key>: {
			$gte: <integer>
		}
	}
)

# less than
db.<collection>.find(
	{
		<interger_key>: {
			$lt: <integer>
		}
	}
)

# less than equals
db.<collection>.find(
	{
		<interger_key>: {
			$lte: <integer>
		}
	}
)
```

## Example working conditionals command
```bash
# Put sample value to test conditionals
db.posts.update(
	{
		title: 'Post Two'
	},
	{
		$set: {
			views: 10
		}
	}
)

# greater than three
db.posts.find(
	{
		views: {
			$gt: 3
		}
	}
)

# greater than equals to three
db.posts.find(
	{
		views: {
			$gte: 3
		}
	}
)

# less than three
db.posts.find(
	{
		views: {
			$lt: 3
		}
	}
)

# less than equals to three
db.posts.find(
	{
		views: {
			$lte: 3
		}
	}
)

# To make it more readable

db.posts.find(
	{
		views: {
			$gt: 3
		}
	}
).pretty 
```
