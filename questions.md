1. What is responsible for defining the routes of the games resource?
express.router() define the routes for the API calls. express.router is initially created within the helpers folder and generic api routes are defined there. The api name i.e. 'game' can then be passed as argument when the router is initialised.

2. What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for?
The client and the server are split, this 

3. The client is used to display/receive data to/from the user/application, whenever the user or client application requires additional data, or needs to alter data that needs to persist through multiple instances it communicates with the server using an api call, the server then interacts with the database. In the instance of games_app, the front end is responsible for taking data from ther user, then using a POST to add the information to the database.

4. What are the the responsibilities of server.js?
server.js is the intermediary from the client side and the database. The api router is initialised here and it takes information provided by users and stores it on the database.

5. What are the responsibilities of the gamesRouter?
It initalises a router for the games API.

6. What process does the the client (front-end) use to communicate with the server?
It uses the api defined by gamesRouter.

7. What optional second argument does the fetch method take? And what is it used for in this application? Hint: See Using Fetch on the MDN docs
These are the API methods that inform server.js what the client wants to do.

8. Which of the games API routes does the front-end application consume (i.e. make requests to)?
Show, delete and create.

9. What are we using the MongoDB Driver for?
If you mean module/node, MongoDB is database for the application and will store data so it can persist through individual sessions.

Extension Why do we need to use ObjectId from the MongoDB driver?
Ids are the safest way to identify and verify that the correct row/entry has been selected. It allows users and the computer to distinguish between duplicate. 