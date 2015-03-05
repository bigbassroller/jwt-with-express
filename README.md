Simple user authentication that useses JavaScript Web Tokens, Bcrypt and Mongodb.

To install:
<pre>git clone https://github.com/bigbassroller/jwt-with-express</pre>

To use you must have node.js and mongodb installed and running.

Start the app with nodemon:
<pre>
nodemon server-auth.js
</pre>

Hit the db with a new user with curl:
<pre>
curl -X POST -d  '{"username": "Larry the Bird", "password": "pass"}' -H "Content-Type: application/json" localhost:3000/user
</pre>

See your users in the mongodb by going into the mongo command line:
<pre>
mongo
</pre>

Use the auth_demo db:
<pre>
use auth_demo
</pre>

See the collections inside the db:
<pre>
show collections
</pre>

See the users created:
<pre>
db.users.find()
</pre>







