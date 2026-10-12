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

HELP: https://blog.e-zest.com/basic-commands-for-mongodb

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


show dbs

<img width="362" height="146" alt="show-dbs" src="https://github.com/user-attachments/assets/e1ea81c9-580f-473a-86b4-98545b8a8c51" />

use sensitive_information

<img width="385" height="52" alt="sensetive mode" src="https://github.com/user-attachments/assets/fac12188-b822-4d5b-b4be-6198e1417096" />

show collections;

<img width="400" height="59" alt="shwo-flag" src="https://github.com/user-attachments/assets/2ecdecc3-91a4-48d6-beb2-1ed637fa94a2" />

db.flag.find()

<img width="468" height="175" alt="flag" src="https://github.com/user-attachments/assets/ba54298b-80fc-4883-8744-487c8efc0d99" />



Answer: db.flag.find()

<img width="632" height="552" alt="Mongod-solved" src="https://github.com/user-attachments/assets/19bb67a4-a95b-4192-879a-4c2905220842" />

