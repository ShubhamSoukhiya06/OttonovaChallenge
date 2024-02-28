# OttonovaChallenge
Project Overview:
The project's primary goal is to retrieve JSON data of multiple cities from the backend and display it on the frontend. It's divided into two main parts:
1.	Server Side (Backend):
      •	The server side is built using Express.js.
      •	Its main function is to provide JSON data containing detailed city information.
      •	The server project's structure includes:
      •	data: Contains city data and related information.
      •	routes: Defines routes for fetching city information.
      •	The server.js file initializes and configures the Express server to only accept GET requests and launches it on port 3001.
      •	Authentication is implemented using a token-based protocol in the routes.js file within the routes folder. Invalid token requests are rejected, ensuring data security.
      •	The ‘/cities’ route, defined in the cities.js file, retrieves city information.
      •	To set up and run the server project:
        o	npm install 
        o	npm start 
      •	Required packages:
        •	cors: Enables Cross-Origin Resource Sharing (CORS) in Express.js, facilitating secure communication between different origins.
        •	express: A minimalist web framework for Node.js, simplifying web application and API development by providing robust HTTP handling, routing, and middleware features.
        •	jsonwebtoken: Facilitates generation, signing, and verification of JSON Web Tokens (JWT) in Node.js applications for secure authentication and authorization.
      •	Navigate to ‘http://localhost:3001/cities’ to verify city data retrieval.

2.	Client Side (Frontend):
    •	The client is built using Angular.
    •	It requests data from the server and renders it for users.
    •	The client project's structure includes:
    •	environments: Defines environment configurations.
    •	model: Contains data models ensuring correct data reception.
    •	services: Defines HTTP requests for server communication. For example, the ‘/cities’ route is used to request data from the backend.
    •	ui: Contains user interface components and views.
    •	The Leaflet map module is used to display cities on a map. Tapping on a marker shows detailed city information.
    •	The default route directs to the cities component on the homepage.
    •	Token exchange occurs during backend requests for added security.
    •	Linting methods are implemented to ensure coding best practices.
    •	Unit tests are written to ensure app functionality.
    •	To set up and run the client project:
      o	npm install 
      o	ng serve 
    •	Navigate to ‘http://localhost:4200’ to view the data.
    •	Run ‘ng test’ to confirm app functionality and successful test execution.
    •	Use ‘ng lint –fix’ for linting staged files before committing to the git repository.

This documentation provides an overview of the project's structure, functionality, setup instructions, and dependencies for both the server-side and client-side components.

![image](https://github.com/ShubhamSoukiya06/OttonovaChallenge/assets/161626798/9e8dc6f1-f787-42e8-8a5a-09de47de8d47)
