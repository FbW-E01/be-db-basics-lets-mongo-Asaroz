# Backend - Database - Basics - Let's MonGO

## Let's monGO

Add your answers directly into this README file.

1. Explain ObjectIDs in MongoDB; what are they?

They are unique identifiers wich MongoDB creates automaticly.

2. You have a collection called "users" with a document like this: `{ _id: 1, name: "Veera" }`. What query would you use to update the name to "Princess Veera Silkenfur"?

db.users.updateOne({ _id: 1, name: "Veera" },{$set:{ _id: 1, name: "Princess Veera Silkenfur" }})

3. How do you make a collection?

db.createCollection("name)

4. So the (old) mongo shell is kind of like a JavaScript REPL. What is a REPL? Which other REPL have we used?

its a programming enviroment that takes in single expressions and gives us back a result in the console. We used Node.

5. So the (old) mongo shell is kind of like a JavaScript REPL. You can use things like variables, try...catch  statements and loops. Experiment with it and find at least three other JavaScript things that we have used that work in the (old) shell. If you can, try to find even more!

https://docs.mongodb.com/v4.4/reference/method/
db.collection.count()
cursor.min()
cursor.map()
db.eval()

6. (Research) So the old shell is pretty cool. How is the new shell better?

The new MongoDB Shell, mongosh, offers numerous advantages over the legacy mongo shell, such as:

Improved syntax highlighting.
Improved command history.
Improved logging.

7. (Research) How can you insert multiple documents at the same time?

we give insertMany() an array of objects.
db.collection.insertMany([{id:1},{id:2},...])


8. (Research) You have a collection called `cats` with a documents like this: `{ name: "Veera" }, { name: "Rauli" }, { name: "BenBen" }` - How can you insert the field `cute: true` into all of them with one command?

db.collection.update({},{$set:{"cute":true}})

9. (Task) Start a timer for 30 minutes. Spend all that time getting to know and reading https://docs.mongodb.com/manual/introduction/ - how far did you get? What was the most cool or interesting thing you learned?
the coolest thing about the documentation was in https://docs.mongodb.com/v4.4/crud/ .
When you go into any of the tabs below(insert documents/query documents/...) you have a small console in there where you can test out every command directly on the website. 
10. Find one SQL Cheatsheet and one MongoDB Cheatsheet and add links to them here.
https://blog.codecentric.de/files/2012/12/MongoDB-CheatSheet-v1_0.pdf
https://learnsql.com/blog/sql-basics-cheat-sheet/


































🌿
