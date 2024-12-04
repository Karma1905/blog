# mern-blog
 # MERN Blog App

A simple blog web application built using the MERN stack (MongoDB, Express, React, and Node.js). The application allows users to create, view, edit, and delete blogs. It features a front page that lists all the registered blogs.

---

## Table of Contents
- Features
- Setup Instructions
- Deployment Process
- Architecture Overview

---

## Features
- **Create** blogs with a title, content, and timestamp.
- **Edit** existing blogs.
- **View** a list of all blogs on the front page.
- **Delete** blogs when no longer needed.

---

## Setup Instructions

### Prerequisites
Ensure the following tools are installed on your system:
- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)
- [Git](https://git-scm.com/)

### Steps
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/mern-blog-app.git
    cd mern-blog-app
    ```
2. Install server dependencies:
    ```bash
    cd server
    npm install
    ```
3. Install client dependencies:
    ```bash
    cd ../client
    npm install
    ```
4. Start MongoDB locally:
    - Ensure MongoDB is running on `localhost:27017`.
    - You can use the following command to start MongoDB (Linux/Mac):
        ```bash
        mongod
        ```
    - For Windows, ensure MongoDB is running from the service manager.

5. Configure environment variables:
    - In the `server` directory, create a `.env` file:
        ```
        MONGO_URI=mongodb://localhost:27017/mern_blog_app
        PORT=5000
        ```
6. Run the application:
    - Start the server:
        ```bash
        cd server
        npm start
        ```
    - Start the client:
        ```bash
        cd ../client
        npm start
        ```

7. Open the app in your browser:
    ```plaintext
    http://localhost:3000
    ```

---

## Deployment Process

### Local Deployment
- Ensure MongoDB is running locally and configured with the correct URI.
- Run both the client and server as detailed in the setup instructions.

### Production Deployment
1. Configure MongoDB for a production database (e.g., MongoDB Atlas).
2. Replace `MONGO_URI` in the `.env` file with the production database URI.
3. Build the React client:
    ```bash
    cd client
    npm run build
    ```
4. Serve the built React app using a Node.js server or a hosting service.

---

## Architecture Overview

### Technology Stack
- **Frontend**: React.js, HTML, CSS, JavaScript
- **Backend**: Node.js, Express.js
- **Database**: MongoDB (local development, scalable to production)

### Folder Structure

