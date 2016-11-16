# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
The back end, or server side, is saved code that remains on the server that can be retrieved later.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
Model
```

Which layer in the MVC pattern communicates with the model?

```bash
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Right now we are only looking at SPAs, so we do not need to integrate several different views (i.e. multiple pages) at this point.
```

What does C.R.U.D stand for?

```bash
Create
Read
Update
Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```bash
Index
Create
Show
Update
Destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
The user uses a client (browser?), which issues a get request to the server
The server then issues a command to the controller to find the index 1 inside 'people'
The controller then issues a request to the model to get the requested data
The model responds to the controller by giving back the data (or an error if data not found)
The controller gives the data to the view
The server then gives the view to the client, where the user can then see the data from the 'GET'
```

What is the command to generate a new rails-api app?

```bash
rails-api new my_api --api
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails server
```

What are the commands to drop, create and migrate a database from the command
line? (3 bullet points)

```bash
bundle exec rake
  db:drop
  db:create
  db:migrate
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bundle exec rails g scaffold pet name:string age:integer
```
