<img width="432" height="146" alt="Screenshot From 2026-10-12 01-03-24" src="https://github.com/user-attachments/assets/1a600fce-8a9f-484a-b0be-e38088919cf4" />

About

Mongod is a very easy Linux machine which introduces the MongoDB database and how to use the MongoDB shell utility to interact with it. Misconfiguring the database by leaving the anonymous user enabled, allows exploitation and full enumeration of the database.

Connecting to MongoDB

curl -O https://downloads.mongodb.com/compass/mongosh-2.3.2-linux-x64.tgz

We must then extract the contents of the tar archive file using the tar utility
tar xvf mongosh-2.3.2-linux-x64.tgz

Navigate to the location where the mongosh binary is present.
cd mongosh-2.3.2-linux-x64/bin

Let's now try to connect to the MongoDB server running on the remote host as an anonymous user.
./mongosh mongodb://{target_IP}:27017

--------------------------------------------------
Task 1
How many TCP ports are open on the machine?

<img width="812" height="311" alt="Mongod-scan" src="https://github.com/user-attachments/assets/550f16d5-3021-4722-8035-d323ede7b4fc" />


Answer: 2

---------------------------------------------------
Task 2

Which service is running on port 27017 of the remote host?
<img width="812" height="311" alt="Mongod-scan" src="https://github.com/user-attachments/assets/8a626c8f-0fb8-40b6-85be-a5d41161e17e" />


Answer: MongoDB 3.6.8

---------------------------------------------------
Task 3
What type of database is MongoDB? (Choose: SQL or NoSQL)


Answer: NoSQL

---------------------------------------------------
Task 4
What command is used to launch the interactive MongoDB shell from the terminal?

mongosh

---------------------------------------------------
Task 5
What is the command used for listing all the databases present on the MongoDB server? (No need to include a trailing ;)

Answer: show dbs

---------------------------------------------------
Task 6
What is the command used for listing out the collections in a database? (No need to include a trailing ;)

Answer: show collections

---------------------------------------------------
Task 7
What command is used to dump the content of all the documents within the collection named flag?


Answer: db.flag.find()
