## Project: City Data Retrieval and Visualization

This project aims to retrieve JSON data of multiple cities from a backend API and display it on a user-friendly frontend. It utilizes Express.js for the server-side and Angular for the client-side.

**To clone the entire project:**

1. Run: `git clone recursive <repository_URL>`

### Overview

- **Project Goal:** Retrieve and visualize city data.
- **Technologies:**
    - Server-side: Express.js
    - Client-side: Angular
    - Additional libraries: Leaflet (map), jsonwebtoken (authentication)

### Server-Side (Backend)

The server is responsible for providing JSON data containing detailed city information. It is built using Express.js and runs on port 3001.

**Structure:**

- `data`: Contains city data and related information.
- `routes`: Defines routes for fetching city information, including authentication using a token-based protocol enforced in `routes.js`.
- `server.js`: Initializes and configures the Express server.

**Setup and Run:**

1. Install dependencies: `npm install`
2. Start the server: `npm start`

**Dependencies:**

- `cors`: Enables Cross-Origin Resource Sharing (CORS) for secure communication.
- `express`: Node.js web framework for building APIs and web applications.
- `jsonwebtoken`: Facilitates generation, signing, and verification of JSON Web Tokens (JWT) for secure authentication.

**Testing:**

Navigate to `http://localhost:3001/cities` to verify data retrieval.

### Client-Side (Frontend)

The client requests data from the server and renders it for users. It is built using Angular and runs on port 4200.

**Structure:**

- `environments`: Defines environment configurations.
- `model`: Contains data models for accurate data reception.
- `services`: Defines HTTP requests for server communication, including fetching city data.
- `ui`: Contains user interface components and views.

**Features:**

- Leverages Leaflet map module to display cities.
- Enables tapping on markers to reveal detailed city information.
- Implements token exchange during backend requests for security.
- Enforces linting methods for code quality.
- Includes unit tests for functionality validation.

**Setup and Run:**

1. Install dependencies: `npm install`
2. Start the development server: `ng serve`

**Testing:**

- Access the application: `http://localhost:4200`
- Run unit tests: `ng test`
- Ensure code quality: `ng lint --fix` (before committing changes)

### Conclusion

This project demonstrates city data retrieval and visualization using Express.js and Angular. It provides a solid foundation for understanding and working with server-side and client-side technologies.
