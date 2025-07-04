# **Introduction** 🚀

Welcome to the **BookStore** project! This application is built using the **MERN stack** and offers a full-stack solution for browsing, managing, and purchasing books along with featured courses. The project is divided into two main parts:

- **Backend**  
  The Backend is developed in **Node.js** using the **Express** framework. It provides RESTful API endpoints that connect to a **MongoDB** database via **Mongoose**. The API allows operations such as retrieving book details and handling user authentication via signup and login functions. In the source files (e.g., Backend/controller/book.controller.js and Backend/controller/user.controller.js fileciteturn0file0 fileciteturn0file1), you can find the controller methods to fetch books and manage user-related operations.

- **Frontend**  
  The Frontend is built with **React** and uses **Vite** as the build tool to optimize the development process. It features components for user interactions including signup, login, course display, and dynamic card components for individual books or courses. Styling is enhanced using **Tailwind CSS** (with DaisyUI components) and additional utility libraries like **react-slick** for carousels, as shown in components such as Freebook.jsx, Cards.jsx, and Navbar.jsx fileciteturn0file3, fileciteturn0file7.

The project follows the standard **MERN** architecture where the Frontend communicates via HTTP requests with the Backend. It is designed to be a responsive web application with a modern user interface empowered by dynamic themes (supporting dark and light modes) and smooth animations.

--------------------------------------------------

# **Requirements** ⚙️

Before running the project, ensure you have the following installed:

| **Requirement**         | **Description**                                                                                                                                                                               |
|-------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Node.js**             | Version 14 or higher is recommended. The Backend is a Node.js application, and its dependencies are managed via npm.                                                                           |
| **MongoDB**             | Install and run MongoDB locally or use a cloud-hosted MongoDB service. The connection URI is provided in the environment variable MongoDBURI (see Backend/index.js fileciteturn0file0).  |
| **npm**                 | Used for installing and managing packages.                                                                                                                                                  |
| **Frontend dependencies** | The Frontend uses React with additional packages like react-router-dom, axios, react-hot-toast, and react-slick. These are listed in the Frontend/package.json fileciteturn0file7.    |
| **Vite**                | For the Frontend build process and live development server. This tool is integrated with React for faster builds and hot module replacement.                                                   |
| **Tailwind CSS & DaisyUI** | For styling the application. The configuration for Tailwind is provided in the postcss.config.js file in the Frontend folder.                                                                  |

### Installation Steps

1. **Clone the repository**
   Code example:
   ```
   git clone https://github.com/harshugarg2907/BookStore.git
   cd BookStore
   ```

2. **Setup the Backend**
   - Navigate to the Backend folder:
     ```
     cd Backend
     ```
   - Install dependencies:
     ```
     npm install
     ```
   - Create a .env file with the required environment variables (e.g., MongoDBURI, PORT).
   - Start the backend server:
     ```
     npm run start
     ```

3. **Setup the Frontend**
   - Open a new terminal and navigate to the Frontend folder:
     ```
     cd Frontend
     ```
   - Install dependencies:
     ```
     npm install
     ```
   - Run the development server:
     ```
     npm run dev
     ```

4. **Testing the Application**
   - Access the Frontend via your web browser (usually at http://localhost:3000 or the port specified by Vite).
   - The application will interact with the Backend API endpoints (e.g., for user signup, login, and fetching book data).

### Additional Notes

- **CORS**  
  The Backend uses the `cors` package to allow requests from the Frontend, ensuring smooth communication between both halves of the application fileciteturn0file0.

- **User Authentication**  
  User authentication is handled using hashed passwords (via bcryptjs) in the Backend. Ensure that any testing environment is set up with appropriate credentials to avoid conflicts.

- **Theming**  
  The Frontend implements dynamic theming with dark and light modes. User preferences are stored in localStorage, thereby allowing a consistent theme experience across sessions.

- **Code Formatting**  
  ESLint configurations are provided in the Frontend (e.g., .eslintrc.cjs) to maintain code consistency and enforce React best practices.

Feel free to explore the source files for a deeper insight into each component and function deployed in this project. Happy coding! 😊

--------------------------------------------------

This README.md serves as a comprehensive guide to get started with the **BookStore** project, highlighting all critical dependencies, setup instructions, and the overall structure of the repository. Enjoy exploring the code!
