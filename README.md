# Backend Project: Contacts, Login, and CRUD Operations

## Description

This project is a **Node.js** and **Express.js** backend application that manages user authentication and CRUD operations for contacts.
Only authenticated users with an access token can perform these operations.

## Technologies Used

 • **Node.js**
 • **Express.js**
 • **MongoDB**
 • **Mongoose**
 • **JSON Web Tokens (JWT)**
 • **bcrypt**
 
# Using the Application

## Steps to Use

1. **Clone the Project:**
   ```bash
   git clone https://github.com/florinmitrana/Node-Express.JS-BackendProject.git
   cd Node-Express.JS-BackendProject
   ```
2. **Install Dependencies**
   ```
   npm install
   ```
3. **Start The Server**
   ```
   npm start
   ```
4. **Use the API's in Postman**
 ```
- Register a User:
  - POST /api/users/register
  - Body: { "username": "your_username", "email": "your_email@example.com", "password": "your_password" }

- Login User:
  - POST /api/users/login
  - Body: { "email": "your_email@example.com", "password": "your_password" }
  - Save the accessToken from the response.

- Authenticated Requests:
  - Add Authorization: Bearer <accessToken> header.

- Create Contact:
  - POST /api/contacts
  - Body: { "name": "contact_name", "email": "contact_email@example.com", "phone": "contact_phone_number" }

- Get Contacts:
  - GET /api/contacts

- Update Contact:
  - PUT /api/contacts/:id
  - Body: { "name": "new_contact_name", "email": "new_contact_email@example.com", "phone": "new_contact_phone_number" }

- Delete Contact:
  - DELETE /api/contacts/:id
```


