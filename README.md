# MongoDB Structure Exercises

## 📄 Description

This repository contains two MongoDB modeling exercises for the Optician Shop *Cul d'Ampolla* project.  
The goal is to design and organize a NoSQL database using MongoDB, representing customers, employees, suppliers, and glasses sales.  

- **Exercise 1**: Client-centered view. Each client contains their data and shopping history.  
- **Exercise 2**: Glasses-centered view. Each glasses model contains its details and the list of clients who bought it.  

## 💻 Technologies Used

- **MongoDB**
- **MongoDB Compass** - GUI for MongoDB
- **Docker** - For local MongoDB container setup
- **Git & GitHub** - Version control
- **Moon Modeler** - For ER diagrams

## 📋 Requirements

- Docker Desktop installed
- MongoDB Compass installed
- Git
- A text editor (e.g., VS Code, Sublime, Notepad++)

## 🛠️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/alaw810/2.3-Databases-MongoDB-Structure.git
   ```

2. Start a MongoDB container with Docker:
   ```bash
   docker run -d --name mongodb -p 27017:27017 -v mongodb_data:/data/db mongo
   ```

3. Open MongoDB Compass and connect to:
   ```
   mongodb://localhost:27017
   ```

4. Create a database for each exercise.

5. Import the `.json` files into your collections.


## 🌐 Deployment

These exercises are intended for local development and learning purposes.  
No deployment to production servers is required.  

If desired, the database can be deployed on:
- MongoDB Atlas (cloud hosting for MongoDB)
- A remote Docker host
