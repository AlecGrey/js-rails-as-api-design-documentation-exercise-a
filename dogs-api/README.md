# Dogs-API

## How to access the resource

To start using the API, first assure all migrations are up-to-date by running `rails db:migrate`, then plant seed data with `rails db:seed`.

Open up your browser and go to `http://localhost:3000/` to access the database.

## Passing search parameters / sorting data

Your search request can have 2 parameters, a **query** and a **sort** parameter.  Format your request as the following: 
```
/dog_search?query=something&sort=something
```
You can omit either of the fields, meaning either of the following are viable searches:
```
/dog_search?query=fido

/dog_search?sort=breed
```

For multi-word queries, be sure to use the `+` symbol in lieu of a space in the HTTP request:
```
/dog_search?query=good+boi
```
