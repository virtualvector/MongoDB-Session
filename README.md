## MongoDB-Session

*   NoSQL Db
*   written in c++
*   Instead of tables we have collections
*   Methods to access collections are avialable for sort insert delete etc..

---------------------------------
### Setting Up

*   Double click on 
> C:\Program Files\MongoDB\Server\4.0\bin\mongod -> for server

> C:\Program Files\MongoDB\Server\4.0\bin\mongo -> for client
*   Create a folder in cd named "data" and subfolder "db" 
*   while closing the client, type 'exit' without quotes

---------------------------------

### using a db

*   In the client console, "show dbs;" -> will show all dbs;
    *   "use abc;" -> uses abc, if abc is not present it will create one

### Creating a collection

*    db.products.insert({pName: 'pepsi', pCategory:'ÇoldDrink', pPrice:25, pQty:30});  -> Creates a collection called products and inserts into it

----------------------------------

## some commands 

- To insert
> db.collectionname.insert();

- To see
> db.collectionname.find();

- Insert using primary key (**_id is like primary key**)
> db.products.insert({_id:501, pName: 'pepsi', pCategory:'ÇoldDrink', pPrice:25, pQty:30});

- Pretty print the data
> db.collectionname.find().pretty();

- where condition, parameter should be in json format only
>  db.collectionname.find({_id:500});  

- Delete operation
> db.collectionname.remove({_id:500});

- Update operation - It overwrites the existing completely
> db.collectionname.update({pName:'pepsi'},{pPrice:45});

- Update operation - without complete override
> db.collectionname.uupdate({_id:500},{**$set:{pCategory:"Nothing Watch"}**})














