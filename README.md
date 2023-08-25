# REQUESTS-IN-POSTMAN

Install the necessary dependencies and then run the start the server in the terminal (npm start), navigate to localhost:8080/api

## Table of Contents

1. [GET REQUEST](#get-request)
2. [DELETE REQUEST](#delete-request)
3. [POST REQUEST](#post-request)
4. [PUT REQUEST](#put-request)
5. [DEPENDENCIES](#dependencies)
6. [REFERENCES](#references)

## GET REQUEST
Syntax

**app.get(path, callback [, callback ...])**

The app.get() request retrieves data to the specified path with specified callback function. A get request only retrieves the data and has no other effect.

**To test the application in postman using a GET request:** 
-  Choose the GET request type;
-  Enter the localhost URL in the tab and click send;
-  In the response bar under the body tab choose to display the response in JSON format.

The response should thereafter provide the response in JSON format.

## DELETE REQUEST
Syntax

**app.delete(path, callback [, callback ...])**
The app.delete() method sends a request to the server to delete the request mentioned in the endpoint. Therefore postman makes it possible to update the server using a DELETE request.
**To test the application in Postman using a DELETE request:**
- Choose the DELETE request type:
- Enter the localhost URL in the tab
- Add projectId as the key parameter and the corresponding value.
- Click send.

The response should display a success message and the object should be removed from the projects.json folder.
## POST REQUEST
Syntax

**app.post(path, callback [, callback ...])**

The POST method is used to add information within the request body to the server.

In postman a POST request allows the adding of data to the endpoint. 
**To test the application in Postman using a POST request:**
- choose the POST request type;
- enter the localhost URL in the post tab;
- click on the body tab below the address bar;
- select option raw and choose JSON from the text dropdown menu;
- enter the object/data to be added to the server using the following key/value pairs: {projectId: number, title: "string", description: "string"};
- Click send;
- In the response bar under the body tab choose to display the response in JSON format.

A success messsage should be displayed in tbe response bar and a new object add in the projects.json file

## PUT REQUEST
Syntax

**app.put(path, callback [, callback ...])**

The put method is used to update/modify a specific piece of data about a specific object on an item on the list.

**To test the application in Postman using a PUT request to update the title:**
- Choose the PUT request type
- Enter http://localhost:8080/api/updateTitle in the tab.
- Click on the body tab under the address bar
- Select option raw and choose JSON from the text dropdown menu;
- Enter the following key/value pairs: {projectId: number, newTitle: "string" }
- Click send
- In the response bar under the body tab choose to display the response in JSON format.

**To test the application in Postman using a PUT request to update the description:**
- Choose the PUT request type
- Enter http://localhost:8080/api/updateDescription in the tab.
- Click on the body tab under the address bar
- Select option raw and choose JSON from the text dropdown menu;
- Enter the following key/value pairs: {projectId: number, newDescription: "string" }
- Click send
- In the response bar under the body tab choose to display the response in JSON format.
A success message should be displayed in the response bar and the description should be updated in the projects.json file.

## DEPENDENCIES

- express (npm i express)
- nodemon (npm i nodemon)
- bodyParser (npm i body-parser)
## REFERENCES

https://www.tutorialspoint.com/how-to-create-a-delete-request-in-postman
https://www.tutorialspoint.com/how-to-create-a-put-request-in-postman
https://www.tutorialspoint.com/how-to-create-a-post-request-in-postman

