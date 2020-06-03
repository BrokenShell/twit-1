# Twit

- HTTP, Client-server architecture; Web Application Routing
- Web Application Views and View Templates
- Adding a database w/ Flask SQL Alchemy

```sh
FLASK_APP=web_app flask db init #> generates app/migrations dir
FLASK_APP=web_app flask db migrate #> creates the db (with "alembic_version" table)
FLASK_APP=web_app flask db upgrade #> creates the specified tables
```

```sh
book_records = Book.query.all()
print(book_records)

new_book = Book(title=request.form["title"], author_id=request.form["author_name"])
db.session.add(new_book)
db.session.commit()
```
