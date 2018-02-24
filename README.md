#Provides CRUD:
* localhost:3000/products
* localhost:3000/categories

## Run
$ mongod
### new tab
$ cd ~/Dev/node/node-rest-api
$ npm start

## CLI REST CRUD commands
### line breaks for view purposes

###Create
curl -i -X POST -H "Content-Type:application.json" -d '{"cat_name":"New Category"}'
 localhost:3000/categories
curl -i -X POST -H "content-type:application/json" -d '{"prod_name":"New Product","prod_desc";"New Product Description","prod_price":3}'
 localhost:3000/products

## Read
curl -i -H "Accept: application/json" localhost:3000/products
curl -i -H "Accept:application.json" localhost:3000/categories

## Update
curl -i -X PUT -H "Content-type: application/json" -d '{ <new values> }' localhost:3000/products/<productID>
curl -i -X PUT -H "content-type:application/json" -d '{<new values>}' localhost:3000/categories/<cateoryID>

## Delete
curl -i -X DELETE localhost:3000/products/<productID>
curl -i -X DELETE localhost:3000/categories/<categorID>

