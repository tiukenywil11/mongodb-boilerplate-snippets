# MongoDB limit commands

## limit command syntax
```bash
db.<collection>.find().limit(<integet>)
```

## Example working limit command
```bash
db.posts.find().limit(2)

# Chain sort and limit
db.posts.find().sort({ title: -1 }).limit(2)

```