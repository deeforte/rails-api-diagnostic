# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
To work with a server that stores info so that we can have functionality such as user IDs, game stats, two users able to use app at once and the information will persist.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
M - model
```

Which layer in the MVC pattern communicates with the model?

```md
C - controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Views are for non-SPA (single page application) apps...which is out dated technology.
```

What does C.R.U.D stand for?

```md
Create, Read, Update and Destroy.
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
routes
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
Index, Show, Create, Update and Destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
client/URL makes a request for people/1
router decides which controller to send the request to
the controller's checks with the model on format of request
the model responds to the request going back to controller
controller gets people/1 from the back end server
controller sends the response to the client
```

What is the command to generate a new rails-api app?

```bash
bin/rails generate scaffold (assuming rails is in the bin directory)
```

What is the command to start an instance of a rails server?

```bash
bin/rake db:create
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
bin/rake db:drop
bin/rake db:create
bin/rake db:migrate
bin/rake db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold pet name:string age:integer
```
