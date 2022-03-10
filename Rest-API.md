Model
- Author

GET all authors
```
GET /authors
```
GET one author information
```
GET /authors/:id
```
EDIT author
```
PUT /authors/:id  (include information)
```



- Book

GET all books
```
GET /books
```

GET a book information
```
GET /books/:id
```

GET all author of a books
```
GET /books/:id/authors
```

Delete a book
```
DELETE /books/:id
```

Delete a author out of a book
```
DELETE /books/:id/authors/:author_id
```

Unpublish a book
```
PUT /books/:id { visible: false }
POST /books/:id/unpublish
```
