# MongoDB intro
## How to create a MongoDB cluster:
1. Create an account on mongodb.com (accounts are free to make).
2. On mongodb.com, navigate to the "Cloud" dropdown menu, and then click on Atlas.
3. Where it says "already have an account? Log in here", click the link and sign in.
4. Under "shared clusters" click "create a cluster". You do not need to pay for a dedicated cluster if you are just using it to learn.
5. Choose your preferred cloud provider and region. This is personal preference.
   Note: if you are starting a cluster for a business, keep in mind that choosing a region that is far from you could cause latency issues.
6. Choose a cluster tier. Everything up to 512 MB of storage is free.
7. Choose a cluster name, and hit "create cluster"
Congratulations! You now have a MongoDB cluster, and you can start creating databases.

## Giving database access to others:
- You can generate a username and password for someone to access your database. This can be done under the database access tab under the security menu by clicking "add new database user".
- You can also whitelist certain IP addresses via the network access tab under the security menu. You are also able to allow access from any IP address by clicking "add IP address" and simply adding 0.0.0.0/0.

## Creating databases and adding data:
- Creating databases can be done either on the shell or in Atlas.
- To create a new database in shell, you can simply use the "use <database name>" command.
- To create a new database in Atlas, simply click the "Create Database" button under the collections tab.
- To create a new database in Compass, navigate to the home page and click the "Create Database" button.
  
## Creating collections within database:
- Collections are a great way to organize documents and keep similar types of data together.
- Creating collections is a very similar process to creating databases- in Atlas and Compass, simply navigate to the database you want to be in and click "create collection".
- In the shell, you can create a new collection within the database you are in with the command "db.createCollection('<collection title>')".
  
## Adding data to your database
- Data is added as JSON objects.
- Data can be added in the MongoDB shell via db.<collection name>.insert() for a single data entry, or db.<collection name>.insertMany() for multiple data entries.
- In Atlas, the "insert document" button allows data can be added in either a pre-formatted JSON object, or it can be added in a terminal using Java notation.
- In Compass, the "add data" button will allow you to either insert a JSON document or upload a .csv or .json file.


## Additional resources that may help you:
- https://www.youtube.com/watch?v=VELru-FCWDM MongoDB Complete Crash Course.
- https://www.youtube.com/watch?v=leNCfU5SYR8 MongoDB Schema Design Best Practices.
- https://www.youtube.com/watch?v=uD3p_rZPBUQ An Introduction to NoSQL databases.
- https://university.mongodb.com/ Free courses provided by MongoDB to help you master and make the most use out of it.
