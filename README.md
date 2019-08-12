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

---------------------------------
*   In the client console, "show dbs;" -> will show all dbs;
    *   "use abc;" -> uses abc, if abc is not present it will create one

### Creating a collection

*    db.products.insert({pName: 'pepsi', pCategory:'ÇoldDrink', pPrice:25, pQty:30});  -> Creates a collection called products and inserts into it




