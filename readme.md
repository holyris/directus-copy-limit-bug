# Repro steps
Start the stack :

```
docker-compose up
```

From another terminal, apply the snapshot :

```
docker-compose exec directus npx directus schema apply ./snapshot.yaml
```

Access the admin : http://localhost:8055

- login: admin@example.com
- password : d1r3ctu5

Import data from the admin in this order : 
- posts
- comments

Update the first post title and save as copy

# Expected behaviour

The copy should have 124 comments, not 100






