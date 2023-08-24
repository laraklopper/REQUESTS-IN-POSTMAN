# REQUESTS-IN-POSTMAN

Install the necessary dependencies and then run the start the server in the terminal (npm start), navigate to localhost:8080/api

## Table of Contents

1. [GET REQUEST](#get-request)
2. [DELETE REQUEST](#delete-request)
3. [POST REQUEST](#post-request)
4. [PUT REQUEST](#put-request)
5. [DEPENDENCIES](#dependencies)

## GET REQUEST
Syntax

**app.get(path, callback [, callback ...])**

The app.get() request retrieves data to the specified path with specified callback function. A get request only retrieves the data and has no other effect.
To test the application in postman using a GET request: choose the request type and enter the localhost URL in the tab and click send.
Choose to display the response in JSON format. The response should thereafter provide the response in JSON format.

## DELETE REQUEST
Syntax

**app.delete(path, callback [, callback ...])**

To delete an object/item by the projectId using the delete method/request in postman choose the request type and enter the localhost URL in the tab and add projectId as the key parameter and the corresponding value as the   
## POST REQUEST
Syntax

**app.post(path, callback [, callback ...])**

The Post method adds an item/object to the list on the server.

## PUT REQUEST
Syntax

**app.put(path, callback [, callback ...])**


The put method is used to update/modify a specific piece of data about a specific object on an item on the list.

## DEPENDENCIES

- express (npm i express)
- nodemon (npm i nodemon)
