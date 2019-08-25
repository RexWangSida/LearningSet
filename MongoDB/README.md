# MongoDB
https://docs.mongodb.com/manual/reference/method/

command line(ubuntu): 
---------------------------
sudo service mongodb start

mongo

shell script:
---------------------------
show dbs //show all databases on local host

show collections //show all collections in current databases

use //create new database or change directory to the exsiting database

db //current database


db.collection.insertOne() //collection of data, table, name is d

db.collection.insertMany()

db.collection.find() //read

db.collection.find(query or projection) //read with specific query, query using {}, 1 and 0 means yes or no

db.product.updateOne() //add feature to the one of the collection. example: db.products.updateOne({_id:1},{$set: {stock:32}})